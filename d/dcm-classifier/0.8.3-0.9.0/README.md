# Comparing `tmp/dcm_classifier-0.8.3.tar.gz` & `tmp/dcm_classifier-0.9.0.tar.gz`

## Comparing `dcm_classifier-0.8.3.tar` & `dcm_classifier-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,619 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.git
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/push_pip.sh
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/requirements_dev.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.github/workflows/push_to_main.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/citations/EndNote_citation.enw
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/citations/RIS_citation.ris
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/citations/bib_citation.bib
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32425 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/src/dcm_classifier/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2203268 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/LICENSE
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/README.md
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 dcm_classifier-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.git
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.gitattributes
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/citations/EndNote_citation.enw
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/citations/RIS_citation.ris
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/citations/bib_citation.bib
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/dcm_classifier.rst
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/_static/dcm-classifier.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/_templates/class.rst
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/_templates/function.rst
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/installation/index.rst
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    21140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    17820 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16172 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_0.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_1.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_10.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_11.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_12.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_13.0.dcm
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_14.0.dcm
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_15.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_16.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_17.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_18.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_19.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_2.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_20.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_21.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_3.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_4.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_5.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_6.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_7.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_8.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_9.0.dcm
+-rw-r--r--   0        0        0    64900 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/all_fields_data/all_fields_file.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm
+-rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm
+-rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm
+-rw-r--r--   0        0        0   218166 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm
+-rw-r--r--   0        0        0   314416 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+-rw-r--r--   0        0        0   314410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm
+-rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm
+-rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm
+-rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm
+-rw-r--r--   0        0        0   314410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm
+-rw-r--r--   0        0        0   166952 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm
+-rw-r--r--   0        0        0   166956 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm
+-rw-r--r--   0        0        0   166946 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm
+-rw-r--r--   0        0        0   166948 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm
+-rw-r--r--   0        0        0   832602 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm
+-rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm
+-rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm
+-rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm
+-rw-r--r--   0        0        0   111700 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm
+-rw-r--r--   0        0        0   111704 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm
+-rw-r--r--   0        0        0   111694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm
+-rw-r--r--   0        0        0   111694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm
+-rw-r--r--   0        0        0   111696 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm
+-rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm
+-rw-r--r--   0        0        0   653404 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm
+-rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm
+-rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm
+-rw-r--r--   0        0        0   653406 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm
+-rw-r--r--   0        0        0   653410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm
+-rw-r--r--   0        0        0   653406 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm
+-rw-r--r--   0        0        0   653410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm
+-rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm
+-rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm
+-rw-r--r--   0        0        0   653404 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm
+-rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm
+-rw-r--r--   0        0        0   653398 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm
+-rw-r--r--   0        0        0   653398 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm
+-rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm
+-rw-r--r--   0        0        0    66392 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm
+-rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm
+-rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm
+-rw-r--r--   0        0        0    66388 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm
+-rw-r--r--   0        0        0    66394 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm
+-rw-r--r--   0        0        0    66382 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm
+-rw-r--r--   0        0        0    66384 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm
+-rw-r--r--   0        0        0    66396 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm
+-rw-r--r--   0        0        0    66382 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm
+-rw-r--r--   0        0        0    66394 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm
+-rw-r--r--   0        0        0   149134 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm
+-rw-r--r--   0        0        0   149132 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm
+-rw-r--r--   0        0        0   149148 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm
+-rw-r--r--   0        0        0   149134 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm
+-rw-r--r--   0        0        0   149114 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm
+-rw-r--r--   0        0        0   149110 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm
+-rw-r--r--   0        0        0   149114 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm
+-rw-r--r--   0        0        0   149110 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm
+-rw-r--r--   0        0        0   234544 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm
+-rw-r--r--   0        0        0   234548 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm
+-rw-r--r--   0        0        0   234538 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm
+-rw-r--r--   0        0        0   234538 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm
+-rw-r--r--   0        0        0   234540 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm
+-rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/flair.xml
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm
+-rw-r--r--   0        0        0   111492 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm
+-rw-r--r--   0        0        0   111492 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm
+-rw-r--r--   0        0        0   832220 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm
+-rw-r--r--   0        0        0   832220 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm
+-rw-r--r--   0        0        0   437476 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm
+-rw-r--r--   0        0        0   132600 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm
+-rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/no_valid_fields.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/emptyBValue.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm
+-rw-r--r--   0        0        0    64842 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm
+-rw-r--r--   0        0        0    64850 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm
+-rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_0.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_1.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_10.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_11.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_12.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_13.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_14.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_15.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_2.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_3.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_4.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_5.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_6.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_7.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_8.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_9.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_0.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_1.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_10.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_11.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_12.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_13.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_14.0.dcm
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_15.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_16.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_17.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_18.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_19.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_2.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_3.0.dcm
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_4.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_5.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_6.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_7.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_8.0.dcm
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_9.0.dcm
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/README.md
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/PKG-INFO
```

### Comparing `dcm_classifier-0.8.3/.pre-commit-config.yaml` & `dcm_classifier-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/CONTRIBUTING.md` & `dcm_classifier-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.9.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/.github/workflows/push_to_main.yml` & `dcm_classifier-0.9.0/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/citations/bib_citation.bib` & `dcm_classifier-0.9.0/citations/bib_citation.bib`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/models/ova_rf_classifier.onnx` & `dcm_classifier-0.9.0/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/models/rf_classifier.onnx` & `dcm_classifier-0.9.0/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.9.0/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/classify_study.py` & `dcm_classifier-0.9.0/scripts/classify_study.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.9.0/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/create_training_sheet.py` & `dcm_classifier-0.9.0/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.9.0/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/modality_classifier_training.py` & `dcm_classifier-0.9.0/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.9.0/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/orientation_model_training.py` & `dcm_classifier-0.9.0/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/run_all_dicom_data_sheets.sh` & `dcm_classifier-0.9.0/scripts/run_all_dicom_data_sheets.sh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/running_classifier.ipynb` & `dcm_classifier-0.9.0/scripts/running_classifier.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990405701754386%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'This tutorial assumes the user has run the testing "*

 * *            'suite and has access to the testing data located in the `tests` directory. This can '*

 * *            'be done by running the following commands in the root directory of the '*

 * *            "repository.')], delete: [2]}}, 2: {'source': ['!git lfs fetch\\n', '!git lfs "*

 * *            "checkout']}}"}*

```diff
@@ -22,24 +22,27 @@
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "source": [
                 "## Setting up the classes\n",
                 "\n",
-                "This tutorial assumes the user has run the testing suite and has access to the testing data located in the `tests` directory. This can be done by running the following command in the root directory of the repository."
+                "This tutorial assumes the user has run the testing suite and has access to the testing data located in the `tests` directory. This can be done by running the following commands in the root directory of the repository."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fc4292140d6c767b",
             "metadata": {},
             "outputs": [],
-            "source": "!pytest"
+            "source": [
+                "!git lfs fetch\n",
+                "!git lfs checkout"
+            ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "327d9c5468193f5d",
             "metadata": {
                 "ExecuteTime": {
```

### Comparing `dcm_classifier-0.8.3/scripts/todo_list` & `dcm_classifier-0.9.0/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/training_config.py` & `dcm_classifier-0.9.0/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/scripts/utilities.py` & `dcm_classifier-0.9.0/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.9.0/src/dcm_classifier/dicom_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 #  =========================================================================
 
 
 """
+Dicom Configuration:
+
+
 List of DICOM header columns that are required for this tool. In the future, the list can be expanded
 or modified as needed.
 
 Those fields were selected experimentally and were deemed useful for the modality and acquisition plane
 classification task, or needed for data organization. Requiring only those fields allows for some flexibility in the
 DICOM header and reduces the dimensionality of the data, thus improving processing efficiency.
 
 Attributes:
-    required_DICOM_fields (tuple): A tuple containing the names of
-    DICOM header columns to be dropped from the dataset.
+    required_DICOM_fields (list[str]): A list of required DICOM fields.
+
+    optional_DICOM_fields (list[str]): A list of optional DICOM fields.
 
-Example:
-    Example usage to drop these columns from a DataFrame:
-    df.drop(columns=required_DICOM_fields, inplace=True)
+    inference_features (list[str]): A list of features that are used for inference.
 """
 
 required_DICOM_fields: list[str] = [
     "StudyInstanceUID",
     "SeriesInstanceUID",
     "SeriesNumber",
     "ImageOrientationPatient",
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.9.0/src/dcm_classifier/dicom_series.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,78 +24,38 @@
 class DicomSingleSeries:
     """
     This class is used to store information about a single DICOM series. It organizes DicomSingleVolumeInfoBase objects
     by series.
 
     Attributes:
         series_number (int): The series number.
-        volume_info_list (List[DicomSingleVolumeInfoBase]): A list to store
-            DicomSingleVolumeInfoBase objects for this series.
-        series_modality (Optional[str]): The modality of the series (e.g., "CT", "MRI").
-        modality_probability (Optional[pd.DataFrame]): A DataFrame containing modality
-            probabilities.
-        acquisition_plane (Optional[str]): The acquisition plane of the series (e.g.,
-            "Sagittal", "Axial").
-        is_isotropic (bool): A flag indicating whether the series is isotropic.
-        has_contrast (bool): A flag indicating whether the series has contrast.
-
-    Methods:
-        get_series_number(self) -> int:
-
-        set_series_modality(self, modality: str) -> None:
-
-        get_series_modality(self) -> str:
-
-        set_modality_probabilities(self, modality_probability: pd.DataFrame) -> None:
-
-        get_modality_probabilities(self) -> pd.DataFrame:
-
-        set_is_isotropic(self, isotropic: bool) -> None:
 
-        get_is_isotropic(self) -> bool:
+        volume_info_list (List[DicomSingleVolumeInfoBase]): A list to store DicomSingleVolumeInfoBase objects for this series.
 
-        set_has_contrast(self, contrast: bool) -> None:
-
-        get_has_contrast(self) -> bool:
-
-        set_acquisition_plane(self, acquisition_plane: str) -> None:
-
-        get_acquisition_plane(self) -> str:
-
-        get_volume_list(self) -> List[DicomSingleVolumeInfoBase]:
+        series_modality (Optional[str]): The modality of the series (e.g., "CT", "MRI").
 
-        add_volume_to_series(self, new_volume_info: DicomSingleVolumeInfoBase) -> None:
+        modality_probability (Optional[pd.DataFrame]): A DataFrame containing modality probabilities.
 
-        organize_volumes(self) -> None:
+        acquisition_plane (Optional[str]): The acquisition plane of the series (e.g., "Sagittal", "Axial").
 
-        get_series_info_dict(self) -> Dict[str, Any]:
+        is_isotropic (bool): A flag indicating whether the series is isotropic.
 
-        get_series_uid(self) -> str:
+        has_contrast (bool): A flag indicating whether the series has contrast.
 
     """
 
     def __init__(
         self,
         series_number: int,
     ) -> None:
         """
         Initialize a DicomSingleSeries instance with the provided series number.
 
         Args:
             series_number (int): The series number associated with this series.
-
-        Attributes:
-            series_number (int): The series number.
-            volume_info_list (List[DicomSingleVolumeInfoBase]): A list to store
-                DicomSingleVolumeInfoBase objects for this series.
-            modality (Optional[str]): The modality of the series (e.g., "t1w", "flair").
-            modality_probability (Optional[pd.DataFrame]): A DataFrame containing modality
-                probabilities.
-            acquisition_plane (Optional[str]): The acquisition plane of the series (e.g.,
-                "Sagittal", "Axial").
         """
         self.series_number: int = series_number
         self.volume_info_list: list[DicomSingleVolumeInfoBase] = list()
         self.series_modality: str = "INVALID"
         self.modality_probability: pd.DataFrame | None = None
         self.acquisition_plane: str = "UNKNOWN"
         self.is_isotropic: bool = False
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.9.0/src/dcm_classifier/dicom_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,35 +25,26 @@
 
 class DicomValidatorBase:
     """
     This is a baseclass with almost no functionality to facilitate the creation of Validator classes for
     specific user projects
 
     Attributes:
-        single_volume_info (DicomSingleVolumeInfoBase): An instance of DicomSingleVolumeInfoBase
-            containing information about a single DICOM volume.
-        _validation_failure_reports (List[str]): A list of validation failure messages.
-
-    Methods:
-        append_to_validation_failure_reports(self, msg: str) -> None:
+        single_volume_info (DicomSingleVolumeInfoBase): An instance of DicomSingleVolumeInfoBase containing information about a single DICOM volume.
 
-        generate_validation_report_str(self, verbose_reporting: bool = False) -> str:
-
-        write_validation_report(self, report_filename_to_append: Optional[Path]) -> None:
+        _validation_failure_reports (List[str]): A list of validation failure messages.
 
-        validate(self) -> bool:
     """
 
     def __init__(self, single_volume_info: DicomSingleVolumeInfoBase) -> None:
         """
         Initialize the DicomValidatorBase.
 
         Args:
-            single_volume_info (DicomSingleVolumeInfoBase): An instance of DicomSingleVolumeInfoBase
-                containing information about a single DICOM volume.
+            single_volume_info (DicomSingleVolumeInfoBase): An instance of DicomSingleVolumeInfoBase containing information about a single DICOM volume.
         """
         self.single_volume_info: DicomSingleVolumeInfoBase = single_volume_info
         self._validation_failure_reports: list[str] = list()
 
     def append_to_validation_failure_reports(self, msg: str) -> None:
         """
         Append a validation failure message to the internal list.
@@ -108,15 +99,15 @@
 
     def write_validation_report(self, report_filename_to_append: Path | None) -> None:
         """
         Write the validation report to a file or print it.
 
         Args:
             report_filename_to_append (Optional[Path]): The filename to write the report to.
-                If None, the report will be printed to the console.
+            If None, the report will be printed to the console.
         """
         msg: str = self.generate_validation_report_str()
 
         if report_filename_to_append is None:
             print(f"{msg}")
         else:
             with open(report_filename_to_append, "a") as vfid:
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.9.0/src/dcm_classifier/dicom_volume.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,88 +42,40 @@
 
 class DicomSingleVolumeInfoBase:
     """
     This class is used to store information about a single DICOM volume.
 
     Attributes:
         one_volume_dcm_filenames (List[Path]): A list of DICOM file paths representing a single volume.
-        ro_user_supplied_dcm_filenames (List[Path]): A list of DICOM file paths representing a single volume.
-        _pydicom_info (pydicom.Dataset): A pydicom.Dataset containing information about the DICOM volume.
-        bvalue (float): The b-value of the DICOM volume.
-        volume_info_dict (Dict[str, Any]): A dictionary containing information about the DICOM volume.
-        itk_image (Optional[FImageType]): The ITK image of the DICOM volume.
-        volume_modality (Optional[str]): The modality of the DICOM volume (e.g., "CT", "MRI").
-        modality_probability (Optional[pd.DataFrame]): A DataFrame containing modality probabilities.
-        acquisition_plane (Optional[str]): The acquisition plane of the DICOM volume (e.g., "Sagittal", "Axial").
-        is_isotropic (Optional[bool]): True if the DICOM volume is isotropic, False otherwise.
-        has_contrast (Optional[bool]): True if the DICOM volume has contrast, False otherwise.
-        parent_series (Optional[DicomSingleSeries]): The parent series of the DICOM volume.
-        volume_index (Optional[int]): The index of the DICOM volume within its series.
-        has_diffusion_gradient (bool): True if the DICOM volume has diffusion gradient, False otherwise.
-
-    Methods:
-        get_volume_series_description(self) -> str:
-
-        set_volume_modality(self, modality: str) -> None:
-
-        get_volume_modality(self) -> str:
-
-        get_series_modality(self) -> str:
-
-        set_is_isotropic(self, isotropic: bool) -> None:
-
-        get_is_isotropic(self) -> bool:
-
-        set_has_contrast(self, contrast: bool) -> None:
-
-        get_has_contrast(self) -> bool:
-
-        get_contrast_agent(self) -> str:
 
-        set_parent_series(self, series) -> None:
-
-        get_parent_series(self):
-
-        set_modality_probabilities(self, modality_probability: pd.DataFrame) -> None:
-
-        get_modality_probabilities(self) -> pd.DataFrame:
-
-        set_acquisition_plane(self, acquisition_plane: str) -> None:
-
-        get_acquisition_plane(self) -> str:
-
-        get_primary_volume_info(self, vol_index: int = 0) -> Dict[str, str]:
-
-        get_itk_image(self) -> FImageType:
-
-        get_series_uid(self) -> str:
+        ro_user_supplied_dcm_filenames (List[Path]): A list of DICOM file paths representing a single volume.
 
-        get_study_uid(self) -> str:
+        _pydicom_info (pydicom.Dataset): A pydicom.Dataset containing information about the DICOM volume.
 
-        get_series_pixel_spacing(self) -> str:
+        bvalue (float): The b-value of the DICOM volume.
 
-        get_series_size(self) -> str:
+        volume_info_dict (Dict[str, Any]): A dictionary containing information about the DICOM volume.
 
-        get_one_volume_dcm_filenames(self) -> List[Path]:
+        itk_image (Optional[FImageType]): The ITK image of the DICOM volume.
 
-        get_volume_dictionary(self) -> Dict[str, Any]:
+        volume_modality (Optional[str]): The modality of the DICOM volume (e.g., "CT", "MRI").
 
-        get_volume_bvalue(self) -> float:
+        modality_probability (Optional[pd.DataFrame]): A DataFrame containing modality probabilities.
 
-        get_series_number(self) -> int:
+        acquisition_plane (Optional[str]): The acquisition plane of the DICOM volume (e.g., "Sagittal", "Axial").
 
-        get_volume_index(self) -> int | None:
+        is_isotropic (Optional[bool]): True if the DICOM volume is isotropic, False otherwise.
 
-        set_volume_index(self, volume_index: int) -> None:
+        has_contrast (Optional[bool]): True if the DICOM volume has contrast, False otherwise.
 
-        is_MR_modality(self):
+        parent_series (Optional[DicomSingleSeries]): The parent series of the DICOM volume.
 
-        _make_one_study_info_mapping_from_filelist(self) -> (str, dict):
+        volume_index (Optional[int]): The index of the DICOM volume within its series.
 
-        get_image_diagnostics(self) -> str:
+        has_diffusion_gradient (bool): True if the DICOM volume has diffusion gradient, False otherwise.
 
     """
 
     def __init__(self, one_volume_dcm_filenames: list[Path | str]) -> None:
         """
         Initializes a DicomSingleVolumeInfoBase instance with a list of DICOM file paths.
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.9.0/src/dcm_classifier/example_image_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     series: DicomSingleSeries, tracew_bval: int = 1000
 ) -> (FImageType, FImageType):
     """
     Compute the trace-weighted image from a diffusion series.
 
     Args:
         series (DicomSingleSeries): The diffusion series.
+
         tracew_bval (int): The preferred b-value for the trace-weighted image.
 
     Returns:
         FImageType: The computed trace-weighted image with pixel type itk.F (float).
     """
     volume_list = series.get_volume_list()
     bval_volumes_dict = {}
@@ -70,14 +71,15 @@
     list_of_raw_bimages: list[FImageType], list_of_bvalues: list[float]
 ) -> FImageType:
     """
     Compute ADC from the min and max b-value images (assumes list_of_images is sorted by ascending b-value).
 
     Args:
         list_of_raw_bimages (List[FImageType]): A list of b-weighted images.
+
         list_of_bvalues (List[float]): A list of b-values.
 
     Returns:
         FImageType: The computed itk ADC image with pixel type itk.F (float).
     """
     # ADC = - (ln(SI_b1) - ln(SI_b2) ) / (b_1 - b_2)
     # ADC = - (ln(SI_b1/SI_b2))/ (b_1 - b_2)
@@ -104,14 +106,15 @@
     """
     Compute ADC from multiple b-value images.
 
     https://www.ajronline.org/doi/full/10.2214/AJR.15.15945?mobileUi=0
 
     Args:
         list_of_raw_bimages (List[FImageType]): A list of b-weighted images.
+
         list_of_bvalues (List[float]): A list of b-values.
 
     Returns:
         FImageType: The computed itk ADC image with pixel type itk.F (float).
     """
 
     list_of_log_images: list[FImageType] = list()
@@ -179,15 +182,17 @@
     recursive_search: bool = True,
 ) -> Path | None:
     """
     Recursively search for files or directories matching a pattern in a base directory.
 
     Args:
         base_dir (Path): The base directory to start the search from.
+
         pattern (str): The pattern to match against.
+
         require_result_type (Optional[str]): If specified, the type of result to require ("f" for file, "d" for directory).
 
     Returns:
         Optional[Path]: The matching result if found, or None if no result or multiple results are found.
     """
 
     glob_obj = base_dir.rglob(pattern) if recursive_search else base_dir.glob(pattern)
@@ -209,15 +214,17 @@
     recursive_search: bool = True,
 ) -> Path | None:
     """
     Recursively search for files or directories matching patterns from a list in a base directory.
 
     Args:
         base_dir (Path): The base directory to start the search from.
+
         patterns (List[str]): The list of patterns to match against.
+
         require_result_type (Optional[str]): If specified, the type of result to require ("f" for file, "d" for directory).
 
     Returns:
         Optional[Path]: The matching result if found, or None if no result or multiple results are found.
     """
     for pattern in patterns:
         candidate = rglob_for_singular_result(
@@ -245,14 +252,15 @@
 
 def compare_RGB_slices(refr_slice_fn: Path, test_slice_fn: Path) -> (int, dict):
     """
     Compare two RGB image slices and count the number of pixels with differences.
 
     Args:
         refr_slice_fn (Path): Filepath to the reference RGB image slice.
+
         test_slice_fn (Path): Filepath to the test RGB image slice.
 
     Returns:
         Tuple[int, Dict[str, FImageType]]: A tuple containing the number of differing pixels
         and a dictionary containing the reference, test, and difference images.
     """
 
@@ -286,17 +294,21 @@
     force_exact_directions: bool,
 ) -> (int, dict, bool):
     """
     Compare two 3D float images and count the number of pixels with differences.
 
     Args:
         refr_fn (Path): Filepath to the reference image.
+
         test_fn (Path): Filepath to the test image.
+
         difference_threshold (float): Threshold for pixel differences.
+
         tolerance_radius (float): Tolerance radius for comparison.
+
         force_exact_directions (bool): Whether to force exact directions in comparison.
 
     Returns:
         Tuple[int, Dict[str, FImageType], bool]: A tuple containing the number of differing pixels,
         a dictionary containing the reference, test, and difference images, and a boolean indicating
         if the images are in the same space.
     """
@@ -346,14 +358,15 @@
     dashes to single dashes. Remove characters that aren't alphanumerics,
     underscores, or hyphens. Convert to lowercase. Also strip leading and
     trailing whitespace, dashes, and underscores.
 
 
     Args:
         value: The string to be converted.
+
         allow_unicode (bool): If True, allows Unicode characters in the slug.
 
     Returns:
         str: The slugified string.
     """
 
     "https://stackoverflow.com/a/295466"
@@ -396,15 +409,17 @@
     inputImage: FImageType, pixel_min: float, pixel_max: float
 ) -> UCImageType:
     """
     Extract the center slice of an input image and perform intensity windowing.
 
     Args:
         inputImage (FImageType): The input itk image with pixel type itk.F (float).
+
         pixel_min (float): Minimum pixel value.
+
         pixel_max (float): Maximum pixel value.
 
     Returns:
         UCImageType: The center slice image with adjusted intensity values.
     """
     extractFilter = itk.ExtractImageFilter[FImageType, FImageType].New()
     extractFilter.SetInput(inputImage)
@@ -476,14 +491,15 @@
 
 def add_itk_images(im1: FImageType, im2: FImageType) -> FImageType:
     """
     Add two input images element-wise.
 
     Args:
         im1 (FImageType): The first input image.
+
         im2 (FImageType): The second input image.
 
     Returns:
         FImageType: The resulting image from adding the two input images element-wise.
     """
     sum_image_filter = itk.AddImageFilter[FImageType, FImageType, FImageType].New()
     sum_image_filter.SetInput1(im1)
@@ -494,14 +510,15 @@
 
 def add_const_to_itk_images(im1: FImageType, offset: float) -> FImageType:
     """
     Add a constant offset to all pixel values in the input image.
 
     Args:
         im1 (FImageType): The input image.
+
         offset (float): The constant offset to be added to each pixel value.
 
     Returns:
         FImageType: The image with the constant offset added to its pixel values.
     """
     sum_image_filter = itk.AddImageFilter[FImageType, FImageType, FImageType].New()
     sum_image_filter.SetInput(im1)
@@ -512,14 +529,15 @@
 
 def sub_itk_images(im1: FImageType, im2: FImageType) -> FImageType:
     """
     Subtract pixel values of the second input image from the first input image element-wise.
 
     Args:
         im1 (FImageType): The first input image.
+
         im2 (FImageType): The second input image.
 
     Returns:
         FImageType: The resulting image from subtracting the pixel values of the second image from the first image.
     """
 
     sub_image_filter = itk.SubtractImageFilter[FImageType, FImageType, FImageType].New()
@@ -531,14 +549,15 @@
 
 def div_itk_images(im1: FImageType, im2: FImageType) -> FImageType:
     """
     Divide pixel values of the first input image by the corresponding pixel values of the second input image element-wise.
 
     Args:
         im1 (FImageType): The first input image.
+
         im2 (FImageType): The second input image.
 
     Returns:
         FImageType: The resulting image from dividing the pixel values of the first image by the second image.
     """
 
     div_image_filter = itk.DivideImageFilter[FImageType, FImageType, FImageType].New()
@@ -550,14 +569,15 @@
 
 def multiply_itk_images(im1: FImageType, scale: float) -> FImageType:
     """
     Multiply all pixel values in the input image by a constant scale.
 
     Args:
         im1 (FImageType): The input image.
+
         scale (float): The constant scale factor to multiply each pixel value.
 
     Returns:
         FImageType: The image with pixel values multiplied by the specified scale factor.
     """
 
     # TODO: Add inplace computations for speed
@@ -592,15 +612,17 @@
     input_image: FImageType, lower_clamp: float, upper_clamp: float = 10**38
 ) -> FImageType:
     """
     Clamp pixel values of an input image within a specified range.
 
     Args:
         input_image (FImageType): The input image.
+
         lower_clamp (float): The lower bound for clamping pixel values.
+
         upper_clamp (float, optional): The upper bound for clamping pixel values. Default is 10^38.
 
     Returns:
         FImageType: The image with pixel values clamped within the specified range.
     """
     cif = itk.ClampImageFilter[FImageType, FImageType].New()
     cif.SetInput(input_image)
@@ -614,14 +636,15 @@
     list_of_images: list[FImageType], list_of_bvalues: list[float]
 ) -> list[FImageType]:
     """
     Multiply a list of images by their corresponding b-values element-wise.
 
     Args:
         list_of_images (List[FImageType]): A list of input images.
+
         list_of_bvalues (List[float]): A list of b-values corresponding to the input images.
 
     Returns:
         List[FImageType]: A list of images with pixel values scaled by their respective b-values.
     """
 
     scaled_by_bvalue_list: list[FImageType] = list()
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.9.0/src/dcm_classifier/image_type_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,63 +50,52 @@
 class ImageTypeClassifierBase:
     """
     Inference class for image type classification. The base implementation is for our standard model. This class
     can be customized by users to implement their own models for targeted for specific datasets.
 
     Attributes:
         classification_model_filename (Union[str, Path]): Path to the classification model file (base implementation requires ONNX file).
-        classification_feature_list (List[str]): List of features used for classification.
-        image_type_map (Dict[str, str]): Mapping between class name and model integer output.
-        min_probability_threshold (float): Minimum probability threshold for classification, defaults to 0.4. If maximum class probability is below this threshold, the image type is set to "unknown".
-
-    Methods:
-        get_min_probability_threshold(self) -> float:
-
-        get_int_to_type_map(self) -> dict:
-
-        _update_diffusion_series_modality(self) -> None:
 
-        check_if_diffusion(self) -> None:
-
-        set_series(self, series: DicomSingleSeries) -> None:
-
-        infer_acquisition_plane(self, feature_dict: dict = None) -> str:
-
-        infer_isotropic(self, feature_dict: dict = None) -> bool | None:
+        classification_feature_list (List[str]): List of features used for classification.
 
-        infer_contrast(self, feature_dict: dict = None) -> bool | None:
+        image_type_map (Dict[str, str]): Mapping between class name and model integer output.
 
-        infer_modality(self, feature_dict: dict = None) -> (str, pd.DataFrame):
+        min_probability_threshold (float): Minimum probability threshold for classification, defaults to 0.4. If maximum class probability is below this threshold, the image type is set to "unknown".
 
-        run_inference(self) -> None:
     """
 
     def __init__(
         self,
-        classification_model_filename: str | Path = dcm_classifier_path
-        / "models"
-        / "ova_rf_classifier.onnx",
+        classification_model_filename: str | Path | None = None,
         classification_feature_list: list[str] = inference_features,
         image_type_map: dict[str, int] = imagetype_to_integer_mapping,
         min_probability_threshold: float = 0.4,
     ):
         """
         Initialize the ImageTypeClassifierBase.
 
         Args:
             classification_model_filename (Union[str, Path]): Path to the classification model file (base implementation requires ONNX file).
+
             classification_feature_list (List[str]): List of features used for classification.
+
             image_type_map (Dict[str, str]): Mapping between class name and model integer output.
+
             mode (str): "series" or "volume" to run inference on series or volume level (a series could have multiple subvolumes).
+
             min_probability_threshold (float): Minimum probability threshold for classification, defaults to 0.4. If maximum class probability is below this threshold, the image type is set to "unknown".
         """
-
-        self.classification_model_filename: str | Path = Path(
-            classification_model_filename
-        )
+        if classification_model_filename is None:
+            self.classification_model_filename = (
+                dcm_classifier_path / "models" / "ova_rf_classifier.onnx"
+            )
+        else:
+            self.classification_model_filename: str | Path = Path(
+                classification_model_filename
+            )
         self.classification_feature_list: list[str] = classification_feature_list
         self.imagetype_to_int_map: dict[str, int] = image_type_map
         self.int_to_imagetype_map: dict[int, str] = self.get_int_to_type_map()
         self.min_probability_threshold: float = min_probability_threshold
         self.series: DicomSingleSeries | None = None
         self.series_number: int | None = None
         self.info_dict: dict[str, Any] | None = None
@@ -189,16 +178,17 @@
                 return "sag"
             else:
                 return "cor"
 
     def infer_isotropic(self, feature_dict: dict = None) -> bool | None:
         """
         Infer the acquisition plane based on DICOM information and image properties.
+
         Args:
-            feature_dict: A dictionary containing features used for classification.
+            feature_dict (dict): A dictionary containing features used for classification.
 
         Returns:
             bool: True if the image is isotropic, False otherwise.
         """
         # TODO: this might need to be changed if acquisition is 3d and spacing has more than 2 values
         # check if the volume was invalidated
         for field in [
@@ -215,16 +205,17 @@
         if np.allclose(spacing, thickness, rtol=0.1):
             return True
         return False
 
     def infer_contrast(self, feature_dict: dict = None) -> bool:
         """
         Infer whether the image has contrast based on DICOM information and image properties.
+
         Args:
-            feature_dict: A dictionary containing features used for classification.
+            feature_dict (dict): A dictionary containing features used for classification.
 
         Returns:
             bool: True if the image has contrast, False otherwise.
         """
         # check if the volume was invalidated
 
         field = "ContrastBolusAgent"
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.9.0/src/dcm_classifier/study_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,39 +27,21 @@
 class ProcessOneDicomStudyToVolumesMappingBase:
     """
     Base class for processing a DICOM study. A study is typically all MRI scans for a single patient's scanning session.
 
     Attributes:
         series_restrictions_list_dwi_subvolumes (List[str]): List of DICOM tags used for filtering DWI sub-volumes.
 
-    Methods:
-        _is_pathlike_object(path_rep: Union[str, Path, PurePath]) -> bool:
+        study_directory (Path): The path to the DICOM study directory as a pathlib Path object.
 
-        __init__(
-            self,
-            study_directory: Union[str, Path],
-            search_series: Optional[Dict[str, int]] = None,
-            inferer: Optional[ImageTypeClassifierBase] = None,
-        ):
-
-        get_list_of_primary_volume_info(self) -> List[Dict[str, str]]:
-
-        get_study_dictionary(self):
-
-        set_inferer(self, inferer: ImageTypeClassifierBase):
+        search_series (Optional[Dict[str, int]]): A dictionary of series to search within the study.
 
-        run_inference(self):
-
-        validate(self):
-
-        __identify_single_volumes(
-            self,
-            study_directory: Path,
-        ) -> Dict[int, DicomSingleSeries]:
+        series_dictionary (Dict[int, DicomSingleSeries]): A dictionary mapping series numbers to DicomSingleSeries objects.
 
+        inferer (Optional[ImageTypeClassifierBase]): An image type classifier for inference.
     """
 
     series_restrictions_list_dwi_subvolumes: list[str] = [
         # https://www.na-mic.org/wiki/NAMIC_Wiki:DTI:DICOM_for_DWI_and_DTI
         # STANDARD
         "0018|9075",  # S 1 Diffusion Directionality
         "0018|9076",  # SQ 1 Diffusion Gradient Direction Sequence
@@ -138,25 +120,22 @@
         Initialize an instance of ProcessOneDicomStudyToVolumesMappingBase.
 
         This constructor sets up the object with the provided parameters, including the study directory,
         search_series dictionary, and optional image type classifier.
 
         Args:
             study_directory (Union[str, Path]): The path to the DICOM study directory.
+
             search_series (Optional[Dict[str, int]]): A dictionary of series to search within the study.
+
             inferer (Optional[ImageTypeClassifierBase]): An image type classifier for inference.
 
         Raises:
             ValueError: If the provided study_directory is not a valid path or path-like object.
 
-        Attributes:
-            study_directory (Path): The path to the DICOM study directory as a pathlib Path object.
-            search_series (Optional[Dict[str, int]]): A dictionary of series to search within the study.
-            series_dictionary (Dict[int, DicomSingleSeries]): A dictionary mapping series numbers to DicomSingleSeries objects.
-            inferer (Optional[ImageTypeClassifierBase]): An image type classifier for inference.
         """
         if ProcessOneDicomStudyToVolumesMappingBase._is_pathlike_object(
             study_directory
         ):
             self.study_directory = Path(study_directory)  # coerce to path object
             del study_directory
         else:
@@ -174,16 +153,15 @@
 
         This method iterates through the series stored in the class's series_dictionary and
         extracts primary volume information from each subseries within those series. It then
         compiles this information into a list of dictionaries, with each dictionary representing
         primary volume information for a single subseries.
 
         Returns:
-            List[Dict[str, str]]: A list of dictionaries containing primary volume information.
-                Each dictionary includes keys and values for primary volume attributes. See get_primary_volume_info function in dicom_volume.py
+            List[Dict[str, str]]: A list of dictionaries containing primary volume information. Each dictionary includes keys and values for primary volume attributes. See get_primary_volume_info function in dicom_volume.py
 
         """
         list_of_volume_info_dictionaries: list[dict[str, str]] = list()
         for (
             series_number,
             series_object,
         ) in self.series_dictionary.items():
@@ -206,17 +184,18 @@
 
         Returns:
             Dict[int, DicomSingleSeries]: A dictionary where keys are series numbers (integers)
             and values are DicomSingleSeries objects containing information about each series.
 
         Example:
             Example usage to retrieve series information:
-            study = ProcessOneDicomStudyToVolumesMappingBase(study_directory_path)
-            study_dict = study.get_study_dictionary()
-            series_info = study_dict.get(1)  # Retrieve information for series number 1
+
+            >>> study = ProcessOneDicomStudyToVolumesMappingBase(study_directory_path)
+            >>> study_dict = study.get_study_dictionary()
+            >>> series_info = study_dict.get(1)  # Retrieve information for series number 1
         """
         return self.series_dictionary
 
     def set_inferer(self, inferer: ImageTypeClassifierBase) -> None:
         """
         Set the image type classifier for inference.
 
@@ -225,17 +204,18 @@
         a class that derives from `ImageTypeClassifierBase`.
 
         Args:
             inferer (ImageTypeClassifierBase): An image type classifier object for inference.
 
         Example:
             Example usage to set an image type classifier:
-            study = ProcessOneDicomStudyToVolumesMappingBase(study_directory_path)
-            image_classifier = MyImageTypeClassifier()  # Replace with your classifier instance
-            study.set_inferer(image_classifier)
+
+            >>> study = ProcessOneDicomStudyToVolumesMappingBase(study_directory_path)
+            >>> image_classifier = MyImageTypeClassifier()  # Replace with your classifier instance
+            >>> study.set_inferer(image_classifier)
         """
         self.inferer = inferer
 
     def run_inference(self) -> None:
         """
         Run inference on each DICOM series using the specified image type classifier.
 
@@ -281,17 +261,18 @@
             - This method uses ITK's GDCMSeriesFileNames to identify series within the study
               based on defined restrictions.
             - Series matching the restrictions are organized into DicomSingleSeries objects
               within the returned dictionary.
 
         Example:
             Example usage to identify and map DICOM series:
-            study = ProcessOneDicomStudyToVolumesMappingBase(study_directory_path)
-            series_mapping = study.__identify_single_volumes(study_directory_path)
-            series_info = series_mapping.get(1)  # Retrieve information for series number 1
+
+            >>> study = ProcessOneDicomStudyToVolumesMappingBase(study_directory_path)
+            >>> series_mapping = study.__identify_single_volumes(study_directory_path)
+            >>> series_info = series_mapping.get(1)  # Retrieve information for series number 1
         """
         namesGenerator = itk.GDCMSeriesFileNames.New()
         namesGenerator.SetUseSeriesDetails(True)
         namesGenerator.SetLoadPrivateTags(True)
         namesGenerator.SetRecursive(True)
         for (
             bvalue_restrictions
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.9.0/src/dcm_classifier/utility_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
     https://dicom.innolitics.com/ciods/enhanced-mr-image/enhanced-mr-image-multi-frame-functional-groups/52009229/00189117/00189087
     NOTE: Bvalue is conditionally required.  This script is to re-inject implied values based on manual inspection or other data sources
 
     `dicom_header_info = dicom.dcmread(dicom_file_name, stop_before_pixels=True)`
 
     Args:
         dicom_header_info: A pydicom object containing DICOM header information.
+
         round_to_nearst_10 (bool): Whether to round the computed b-value to the nearest 10. (i.e. bvalues of 46,47,48,49,50,51,52,53,54,55 are reported as 50)
 
     Returns:
         float: The computed or extracted b-value.
     """
 
     # bvalue tags from private fields provided by https://www.nmr.mgh.harvard.edu/~greve/dicom-unpack
@@ -239,14 +240,15 @@
 
 
 def get_diffusion_gradient_direction(
     dicom_header_info: pydicom.Dataset,
 ) -> np.ndarray | None:
     """
     Extract the diffusion gradient direction from DICOM header information.
+
     Args:
         dicom_header_info: pydicom.Dataset object containing header information.
 
     Returns:
         numpy array containing the diffusion gradient direction.
     """
     private_tags_map = collections.OrderedDict(
@@ -336,14 +338,15 @@
 
 def vprint(msg: str, verbose: bool = False) -> None:
     """
     Conditionally print a message if the 'verbose' flag is set.
 
     Args:
         msg (str): The message to print.
+
         verbose (bool, optional): Whether to print the message. Default is False.
     """
     if verbose:
         print(msg)
 
 
 def sanitize_dicom_dataset(
@@ -352,15 +355,17 @@
     optional_info_list: list[str],
 ) -> tuple[dict, bool]:
     """
     Validates the DICOM fields in the DICOM header to ensure all required fields are present.
 
     Args:
         ro_dataset (pydicom.Dataset): The input DICOM dataset.
+
         required_info_list (list[str]): A list of required DICOM fields.
+
         optional_info_list (list[str]): A list of optional DICOM fields.
 
     Returns:
         tuple[dict, bool]: A dictionary containing the sanitized DICOM fields and a boolean indicating whether the validation was successful.
 
     Raises an exception if any required fields are missing.
     """
@@ -712,14 +717,15 @@
 
 def convert_array_to_min_max(name: str, value_list: list[int]) -> list:
     """
     Compute the minimum and maximum values of a DICOM array field.
 
     Args:
         name: Original DICOM field name.
+
         value_list: Original DICOM list values.
 
     Returns:
         list: A list of (name, value) pairs representing the minimum and maximum values.
     """
 
     name = name.replace(" ", "")
@@ -731,14 +737,15 @@
 
 def convert_array_to_index_value(name: str, value_list: MultiValue | ndarray) -> list:
     """
     Takes a DICOM array and expands it to an indexed list of values.
 
     Args:
         name: Original DICOM field name.
+
         value_list: Original DICOM list values.
 
     Returns:
         A list of (name, value) pairs, where each value in the original list is indexed with a unique name.
     """
     # If value is a multi-value field, then break it apart
     multi_value_list = value_list
```

### Comparing `dcm_classifier-0.8.3/src/dcm_classifier/models/ova_rf_classifier.onnx` & `dcm_classifier-0.9.0/src/dcm_classifier/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/tests/conftest.py` & `dcm_classifier-0.9.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,33 +14,25 @@
 current_file_path: Path = Path(__file__).parent
 inference_model_path = list(
     Path(__file__).parent.parent.rglob("models/rf_classifier.onnx")
 )[0]
 
 # path to the testing data directory
 test_data_dir_path: Path = Path(__file__).parent / "testing_data"
-tar_path: Path = test_data_dir_path / "anonymized_testing_data.tar.gz"
 
 # path to the anonymized testing data directory
 testing_dicom_dir: Path = test_data_dir_path / "anonymized_testing_data"
 
-# Check to see if tar file is unpacked or not
-if not testing_dicom_dir.exists():
-    testing_dicom_dir.mkdir(parents=True)
-    subprocess.run(f"tar -xf {tar_path} -C {test_data_dir_path}", shell=True)
-
 # run study on anonymized data
 inferer = ImageTypeClassifierBase(classification_model_filename=inference_model_path)
 study = ProcessOneDicomStudyToVolumesMappingBase(
     study_directory=(testing_dicom_dir / "anonymized_data"), inferer=inferer
 )
 study.run_inference()
 
-s_test = study.series_dictionary.get(15)
-print(s_test.get_volume_list()[0].get_one_volume_dcm_filenames()[0])
 
 ax_series = [
     study.series_dictionary.get(6),
     study.series_dictionary.get(7),
     # study.series_dictionary.get(8),
     # study.series_dictionary.get(9),
     study.series_dictionary.get(11),
```

### Comparing `dcm_classifier-0.8.3/tests/testing_data/mock_data.txt` & `dcm_classifier-0.9.0/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.9.0/tests/unit_testing/test_dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.9.0/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.9.0/tests/unit_testing/test_dicom_volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,39 +124,24 @@
 def test_get_modality(mock_volumes):
     volume_info = DicomSingleVolumeInfoBase(mock_volumes[0])
     assert volume_info.get_volume_modality() == "INVALID"
     volume_info.set_volume_modality("fa")
     assert volume_info.get_volume_modality() == "fa"
 
 
-@pytest.mark.skip(reason="Not implemented yet")
-def test_set_modality_probabilities(mock_volumes):
-    probabilities = pd.DataFrame(
-        data={"case1": 0.4, "case2": 0.3, "case3": 0.75}, index=["t1w", "flair", "t2w"]
-    )
-    vol = DicomSingleVolumeInfoBase(mock_volumes[0])
-    vol.set_modality_probabilities(probabilities)
-    assert vol.get_modality_probabilities().aggregate == probabilities
-
-
 def test_no_files_provided():
     with pytest.raises(ValueError) as ex:
         _ = DicomSingleVolumeInfoBase([])
     assert "No file names provided list" in str(ex.value)
 
 
 def test_invalid_volume_modality(mock_volumes):
     assert DicomSingleVolumeInfoBase(mock_volumes[0]).get_volume_modality() == "INVALID"
 
 
-@pytest.mark.skip(reason="Not implemented yet")
-def test_get_modality_probabilities():
-    pass
-
-
 # Test asserts false because the mock volume has a flair modality but that is an MR modality...
 def test_is_MR_modality(mock_volume_study):
     for series_num, series in mock_volume_study.get_study_dictionary().items():
         for volume in series.get_volume_list():
             assert volume.is_MR_modality() is False
```

### Comparing `dcm_classifier-0.8.3/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.9.0/tests/unit_testing/test_study_processing.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,31 +44,15 @@
 #     study_to_volume_mapping_base = ProcessOneDicomStudyToVolumesMappingBase(study_path)
 #     volume_info_dictionaries = (
 #         study_to_volume_mapping_base.get_list_of_primary_volume_info()
 #     )
 #     assert len(volume_info_dictionaries) == 13
 
 
-@pytest.mark.skip(reason="Need to add public data")
-def test_get_list_of_primary_volume_info_with_search_series():
-    test_data_dicom_dir: str = "XXXX"
-    study_path = relative_testing_data_path / test_data_dicom_dir
-    study_to_volume_mapping_base = ProcessOneDicomStudyToVolumesMappingBase(
-        study_path, {"test": 7}
-    )
-    volume_info_dictionaries = (
-        study_to_volume_mapping_base.get_list_of_primary_volume_info()
-    )
-    assert len(volume_info_dictionaries) == 4
-
-
-# @pytest.mark.skip(reason="Need to add public data")
 def test_get_study_dictionary_and_set_inferer():
-    # test_data_dicom_dir: str = "XXXX"
-    # study_path = relative_testing_data_path / test_data_dicom_dir
     study_path = (
         relative_testing_data_path / "anonymized_testing_data" / "anonymized_data"
     )
 
     default_classification_model_filename: Path = (
         Path(__file__).parents[2] / "models" / "rf_classifier.onnx"
     )
```

### Comparing `dcm_classifier-0.8.3/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.9.0/tests/unit_testing/test_utility_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,44 +66,19 @@
     assert results == [
         "dwi-series-number-006-index-01",
         "DWI-series-number-006-index-01",
         "dwi-series-nùmber-006-index-01",
     ]
 
 
-@pytest.mark.skip(reason="Not implemented yet")
-def test_cmd_exists():
-    pass
-
-
-@pytest.mark.skip(reason="Not implemented yet")
-def test_compare_rgb_slices():
-    pass
-
-
-@pytest.mark.skip(reason="Not implemented yet")
+@pytest.mark.skip(reason="Not implemented yet, need more test data")
 def test_get_bvalue():
     pass
 
 
-@pytest.mark.skip(reason="Not implemented yet")
-def test_get_min_max():
-    pass
-
-
-@pytest.mark.skip(reason="Not implemented yet")
-def test_get_coded_dictionary_elements():
-    pass
-
-
-@pytest.mark.skip(reason="Not implemented yet")
-def test_exp_image():
-    pass
-
-
 def test_vprint(capsys):
     assert vprint("test", True) is None
 
     captured = capsys.readouterr()
     assert captured.out == "test\n"
 
 
@@ -247,15 +222,23 @@
             "SeriesInstanceUID",
             "FileName",
             "list_of_ordered_volume_files",
         ]
     ]
 
     # assert the fields that are in the dataset are set to one of these invalid values
-    invalid_fields = ["INVALID_VALUE", "-12345", "Unknown", "-12345.0", "None", ""]
+    invalid_fields = [
+        "INVALID_VALUE",
+        "-12345",
+        "Unknown",
+        "-12345.0",
+        "None",
+        "",
+        "000000.00",
+    ]
     for field in all_fields:
         print(field, ds_dict[field])
         if "unknown" in ds_dict[field].lower():
             assert True
         else:
             assert ds_dict[field] in invalid_fields
```

### Comparing `dcm_classifier-0.8.3/.gitignore` & `dcm_classifier-0.9.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 
 # Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,latex,c,c++
 # Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,latex,c,c++
 
 # test files
-tests/testing_data/anonymized_testing_data/**
 pytest.xml
 pytest-coverage.txt
 
 # data files
 *.xlsx
 *.pkl
 
 # image files
 *.nii.gz
-# dicom files
-*.dcm
+
 
 # directories
 **/cnn_logs
 **/.idea
 **/__pycache__
 
 ### C ###
```

### Comparing `dcm_classifier-0.8.3/LICENSE` & `dcm_classifier-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.3/README.md` & `dcm_classifier-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,15 +74,25 @@
 
 or pass the path to a separate model
 
 `$ python3 <path_to_scripts_directory>/classify_study.py -m models/ova_rf_classifier.onnx -d <path_to_dicom_session>`
 
 ### Testing
 
-Testing in the dcm-classifier package is done using pytest. To run the tests, navigate to the root directory of the package and run the following command:
+Testing in the dcm-classifier package is done using pytest. To run the tests, navigate to the root directory of the package
+
+The testing data is stored in Git LFS so the following commands will be needed before running pytest
+
+```bash
+  git lfs fetch
+  git lfs checkout
+```
+
+and now
+
 ```bash
   pytest
   # or to fail on warnings
   python3 -Werror::FutureWarning -m pytest
 ```
 ### Coverage Analysis
```

### Comparing `dcm_classifier-0.8.3/pyproject.toml` & `dcm_classifier-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.8.3'
+version = '0.9.0'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
   { name="Cavan Riley", email="cavan-riley@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
```

### Comparing `dcm_classifier-0.8.3/PKG-INFO` & `dcm_classifier-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.8.3
+Version: 0.9.0
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>, Cavan Riley <cavan-riley@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: itk-core>=5.3.0
@@ -96,15 +96,25 @@
 
 or pass the path to a separate model
 
 `$ python3 <path_to_scripts_directory>/classify_study.py -m models/ova_rf_classifier.onnx -d <path_to_dicom_session>`
 
 ### Testing
 
-Testing in the dcm-classifier package is done using pytest. To run the tests, navigate to the root directory of the package and run the following command:
+Testing in the dcm-classifier package is done using pytest. To run the tests, navigate to the root directory of the package
+
+The testing data is stored in Git LFS so the following commands will be needed before running pytest
+
+```bash
+  git lfs fetch
+  git lfs checkout
+```
+
+and now
+
 ```bash
   pytest
   # or to fail on warnings
   python3 -Werror::FutureWarning -m pytest
 ```
 ### Coverage Analysis
```

