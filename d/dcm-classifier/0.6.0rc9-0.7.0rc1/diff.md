# Comparing `tmp/dcm_classifier-0.6.0rc9.tar.gz` & `tmp/dcm_classifier-0.7.0rc1.tar.gz`

## Comparing `dcm_classifier-0.6.0rc9.tar` & `dcm_classifier-0.7.0rc1.tar`

### file list

```diff
@@ -1,48 +1,52 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/.git
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/push_pip.sh
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/requirements.txt
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/requirements_dev.txt
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/models/rf_classifier.onnx
--rwxr-xr-x   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/anonymize_dicom_directory.py
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/classify_study.py
--rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/combine_excel_spreadsheets.py
--rwxr-xr-x   0        0        0    22411 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/create_dicom_fields_sheet.py
--rwxr-xr-x   0        0        0     4629 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/dir_to_xlsx.py
--rwxr-xr-x   0        0        0     2649 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/edit_dcm_files.py
--rwxr-xr-x   0        0        0     8606 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/merge_excel_files.py
--rwxr-xr-x   0        0        0    14178 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/modality_classifier_training.py_backup
--rwxr-xr-x   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/organize_dicom_to_bids.py
--rwxr-xr-x   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/override_study_UIDs.py
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/pydicom_info_cache.py
--rwxr-xr-x   0        0        0     1564 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/run_all_predict_hd.sh
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/scripts/todo_list
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    17858 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    18118 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    30553 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2032345 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/unit_testing/test_dicom_data.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/unit_testing/test_namic_dicom_typing.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/LICENSE
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/README.md
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/pyproject.toml
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dcm_classifier-0.6.0rc9/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.git
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/push_pip.sh
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/requirements_dev.txt
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/anonymized_testing_data.tar.gz
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11288 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/README.md
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/PKG-INFO
```

### Comparing `dcm_classifier-0.6.0rc9/.pre-commit-config.yaml` & `dcm_classifier-0.7.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/models/ova_rf_classifier.onnx` & `dcm_classifier-0.7.0rc1/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/models/rf_classifier.onnx` & `dcm_classifier-0.7.0rc1/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.7.0rc1/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/scripts/classify_study.py` & `dcm_classifier-0.7.0rc1/scripts/classify_study.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 
 import argparse
 import sys
 from typing import Any
 import pandas as pd
 import tabulate
 from collections import OrderedDict as ordered_dict
-
-# warnings.simplefilter(action="ignore", category=FutureWarning)
+from pathlib import Path
 
 try:
     from dcm_classifier.study_processing import ProcessOneDicomStudyToVolumesMappingBase
     from dcm_classifier.image_type_inference import ImageTypeClassifierBase
 except Exception as e:
-    from pathlib import Path
-
     print(f"Missing module import {e}")
     print(
         f"Try setting export PYTHONPATH={Path(__file__).parent.parent.as_posix()}/src"
     )
     sys.exit(255)
 
 
@@ -26,95 +23,121 @@
     return "|" + ("-" * (column_width + 2) + "|") * 4
 
 
 def generate_row(*args, column_width):
     return "| " + " | ".join(arg.ljust(column_width) for arg in args) + " |"
 
 
-# Set up argparse
-description = (
-    "Authors: Michal Brzus, Hans J. Johnson\n"
-    "Classify image modality and acquisition plane of DICOM MR data by series and volumes.\n"
-)
-parser = argparse.ArgumentParser(description=description)
-parser.add_argument(
-    "-d",
-    "--session_directory",
-    required=True,
-    help="Path to the patient session directory with dicom data",
-)
-parser.add_argument(
-    "-m",
-    "--model",
-    required=True,
-    help="Path to the model used for image type inference",
-)
-
-args = parser.parse_args()
-
-print(description)
-inferer = ImageTypeClassifierBase(classification_model_filename=args.model)
-study = ProcessOneDicomStudyToVolumesMappingBase(
-    study_directory=args.session_directory, inferer=inferer
-)
-study.run_inference()
-
-list_of_inputs: list[dict[str, Any]] = []
-list_of_probabilities: list[pd.DataFrame] = []
-list_of_dictionaries: list[dict[str, str]] = []
-
-for series_number, series in study.series_dictionary.items():
-    for index, volume in enumerate(series.get_volume_list()):
-        # modality = volume.get_modality()
-        #         plane = volume.get_acquisition_plane()
-        #         print(generate_row(str(series_number), modality, plane, iso, column_width=col_width))
-        current_dict: dict[str, str] = ordered_dict()
-        current_dict["Series#"] = str(series_number)
-        current_dict["Vol.#"] = str(volume.get_volume_index())
-        current_dict["Volume Modality"] = str(volume.get_volume_modality())
-        current_dict["Series Modality"] = str(series.get_series_modality())
-        current_dict["Acq.Plane"] = str(volume.get_acquisition_plane())
-        current_dict["Isotropic"] = str(volume.get_is_isotropic())
-        print(volume.get_modality_probabilities().to_string(index=False))
-        current_dict["Bvalue"] = str(volume.get_volume_bvalue())
-        current_dict["SeriesDesc"] = volume.get_volume_series_description()
-        # info_dict = series.get_series_info_dict()
-        inputs_df: dict[str, Any] = volume.get_volume_dictionary()
-        current_dict["ImageType"] = str(inputs_df.get("ImageType", "Unknown"))
-        for unwanted in [
-            "FileName",
-            "StudyInstanceUID",
-            "SeriesInstanceUID",
-            "list_of_ordered_volume_files",
-        ]:
-            if unwanted in inputs_df:
-                inputs_df.pop(unwanted)
-
-        list_of_inputs.append(inputs_df)
-
-        prob_df: pd.DataFrame = volume.get_modality_probabilities()
-        list_of_probabilities.append(prob_df)
-        list_of_dictionaries.append(current_dict)
-
-
-df: pd.DataFrame = pd.DataFrame(list_of_dictionaries)
-df.sort_values(by=["Series#", "Vol.#"], inplace=True)
-
-table_msg: str = tabulate.tabulate(df, headers="keys", tablefmt="psql", showindex=False)
-print(table_msg)
-
-# all_inputs_df: pd.DataFrame = pd.DataFrame(list_of_inputs)
-# inputs_msg: str = tabulate.tabulate(
-#     all_inputs_df, headers="keys", tablefmt="psql", showindex=False
-# )
-# print(inputs_msg)
-#
-# all_prob_df: pd.DataFrame = pd.concat(list_of_probabilities, axis=0, ignore_index=True)
-# prob_msg: str = tabulate.tabulate(
-#     all_prob_df, headers="keys", tablefmt="psql", showindex=False
-# )
-# print(prob_msg)
+def main():
+    # Set up argparse
+    description = (
+        "Authors: Michal Brzus, Hans J. Johnson\n"
+        "Classify image modality and acquisition plane of DICOM MR data by series and volumes.\n"
+    )
+    parser = argparse.ArgumentParser(description=description)
+    parser.add_argument(
+        "-d",
+        "--session_directory",
+        required=True,
+        help="Path to the patient session directory with dicom data",
+    )
+    parser.add_argument(
+        "-m",
+        "--model",
+        required=True,
+        help="Path to the model used for image type inference",
+    )
+    parser.add_argument(
+        "-n",
+        "--nifti_dir",
+        required=False,
+        default=None,
+        help="Path to the directory where the NIFTI files are stored for each volume",
+    )
+
+    args = parser.parse_args()
+
+    nifti_dir: Path | None = Path(args.nifti_dir) if args.nifti_dir else None
+    if nifti_dir:
+        import itk
+
+        nifti_dir.mkdir(parents=True, exist_ok=True)
+
+    print(description)
+    inferer = ImageTypeClassifierBase(classification_model_filename=args.model)
+    study = ProcessOneDicomStudyToVolumesMappingBase(
+        study_directory=args.session_directory, inferer=inferer
+    )
+    study.run_inference()
+
+    list_of_inputs: list[dict[str, Any]] = []
+    list_of_probabilities: list[pd.DataFrame] = []
+    list_of_dictionaries: list[dict[str, str]] = []
+
+    for series_number, series in study.series_dictionary.items():
+        for index, volume in enumerate(series.get_volume_list()):
+            current_dict: dict[str, str] = ordered_dict()
+            current_dict["Series#"] = str(series_number)
+            current_dict["Vol.#"] = str(volume.get_volume_index())
+            current_dict["Volume Modality"] = str(volume.get_volume_modality())
+            current_dict["Series Modality"] = str(series.get_series_modality())
+            current_dict["Acq.Plane"] = str(volume.get_acquisition_plane())
+            current_dict["Isotropic"] = str(volume.get_is_isotropic())
+            print(volume.get_modality_probabilities().to_string(index=False))
+            current_dict["Bvalue"] = str(volume.get_volume_bvalue())
+            try:
+                current_dict["SeriesDesc"] = volume.get_volume_series_description()
+            except AttributeError as e:
+                current_dict["SeriesDesc"] = "None"
+            inputs_df: dict[str, Any] = volume.get_volume_dictionary()
+            current_dict["ImageType"] = str(inputs_df.get("ImageType", "Unknown"))
+            for unwanted in [
+                "FileName",
+                "StudyInstanceUID",
+                "SeriesInstanceUID",
+                "list_of_ordered_volume_files",
+            ]:
+                if unwanted in inputs_df:
+                    inputs_df.pop(unwanted)
+
+            list_of_inputs.append(inputs_df)
+
+            prob_df: pd.DataFrame = volume.get_modality_probabilities()
+            list_of_probabilities.append(prob_df)
+            list_of_dictionaries.append(current_dict)
+            if nifti_dir is not None:
+                bvalue_suffix: str = (
+                    f"_b{volume.get_volume_bvalue()}"
+                    if volume.get_volume_bvalue() >= 0
+                    else ""
+                )
+                image_file_name: str = (
+                    f"{series_number:04}_{volume.get_volume_index():03}"
+                    f"_{volume.get_series_modality()}{bvalue_suffix}.nii.gz"
+                )
+                itk_image = volume.get_itk_image()
+                itk.imwrite(itk_image, nifti_dir / image_file_name)
+
+    df: pd.DataFrame = pd.DataFrame(list_of_dictionaries)
+    df.sort_values(by=["Series#", "Vol.#"], inplace=True)
+
+    table_msg: str = tabulate.tabulate(
+        df, headers="keys", tablefmt="psql", showindex=False
+    )
+    print(table_msg)
+
+    # all_inputs_df: pd.DataFrame = pd.DataFrame(list_of_inputs)
+    # inputs_msg: str = tabulate.tabulate(
+    #     all_inputs_df, headers="keys", tablefmt="psql", showindex=False
+    # )
+    # print(inputs_msg)
+    #
+    # all_prob_df: pd.DataFrame = pd.concat(list_of_probabilities, axis=0, ignore_index=True)
+    # prob_msg: str = tabulate.tabulate(
+    #     all_prob_df, headers="keys", tablefmt="psql", showindex=False
+    # )
+    # print(prob_msg)
 
 
 if __name__ == "__main__":
     # Execute the script
-    pass  # The main logic is already written above, so this is just a placeholder.
+    main()
```

### Comparing `dcm_classifier-0.6.0rc9/scripts/modality_classifier_training.py_backup` & `dcm_classifier-0.7.0rc1/scripts/orientation_model_training.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,330 +1,262 @@
+#!/usr/bin/env python3
+
 import numpy as np
 import matplotlib.pyplot as plt
-from matplotlib import rcParams
 import pandas as pd
 from sklearn import metrics
 from sklearn.ensemble import RandomForestClassifier
+from sklearn.model_selection import train_test_split  # Import train_test_split function
 from sklearn.tree import DecisionTreeClassifier  # Import Decision Tree Classifier
-from sklearn.metrics import ConfusionMatrixDisplay
+from sklearn.metrics import ConfusionMatrixDisplay, classification_report
 from sklearn.tree import export_graphviz
-from sklearn.model_selection import KFold
 
-import time
 from io import StringIO
 
 # from IPython.display import Image
 import pydotplus
 from skl2onnx import convert_sklearn
 from skl2onnx.common.data_types import FloatTensorType
 import onnxruntime as rt
 
-from .create_dicom_fields_sheet import make_unique_ordered_list
-
+from .create_dicom_fields_sheet.py import make_unique_ordered_list
 
-rcParams.update({"figure.autolayout": True})
 
 # overwrite objects for new data modalities
-imagetype_to_integer_mapping = {
-    "adc": 0,
-    "fa": 1,
-    "tracew": 2,
-    "t2w": 3,
-    "t2starw": 4,
-    "t1w": 5,
-    "flair": 6,
-    "field_map": 7,
-    "dwig": 8,
-    "dwi_multishell": 9,
-    "fmri": 10,
+plane_to_integer_mapping = {
+    "ax": 0,
+    "cor": 1,
+    "sag": 2,
 }
 
-modality_columns = [
-    "ImageTypeADC",
-    "ImageTypeFA",
-    "ImageTypeTrace",
-    "SeriesVolumeCount",
-    "EchoTime",
-    "RepetitionTime",
-    "FlipAngle",
-    "PixelBandwidth",
-    "SAR",
-    "Diffusionb-valueCount",
-    "Diffusionb-valueMax",
+# modify columns to exclude the orientation
+# the decision tree for acqusition plane (in create_labels.py) takes care of that
+plane_cols = [
+    "ImageOrientationPatient_0",
+    "ImageOrientationPatient_1",
+    "ImageOrientationPatient_2",
+    "ImageOrientationPatient_3",
+    "ImageOrientationPatient_4",
+    "ImageOrientationPatient_5",
 ]
 
 
-def generate_training_data(label_dataframe: str, dicom_dataframe: str, name: str):
-    """
-    Generate data for model training. Function modifies the "everything" DICOM dataframe by injecting labels from
-    label_dataframe.
-    :param label_dataframe: filepath to the label dataframe
-    :param dicom_dataframe: filepath of "everything" dicom dataframe
-    :return:
-        x - training data
-        y - labels
-    """
-    input_output_training_columns = modality_columns + ["SeriesInstanceUID", "Modality"]
-
-    label_df = pd.read_excel(label_dataframe)
-    dicom_df = pd.read_excel(dicom_dataframe)
-
-    df = pd.merge(dicom_df, label_df, on="SeriesInstanceUID")
-    pima = pd.DataFrame(df[input_output_training_columns])
-
-    pima = pima[
-        (pima["Modality"] == "adc")
-        | (pima["Modality"] == "fa")
-        | (pima["Modality"] == "tracew")
-        | (pima["Modality"] == "t2w")
-        | (pima["Modality"] == "t2starw")
-        | (pima["Modality"] == "t1w")
-        | (pima["Modality"] == "flair")
-        | (pima["Modality"] == "field_map")
-        | (pima["Modality"] == "dwig")
-        | (pima["Modality"] == "dwi_multishell")
-        | (pima["Modality"] == "fmri")
-    ]
-
-    pima["Modality"].replace(imagetype_to_integer_mapping, inplace=True)
-    pima["Modality"] = pima["Modality"].astype(int)
-    pima["Modality"] = pima["Modality"].astype("category")
-
-    model_generation_df = pd.DataFrame(pima[input_output_training_columns])
-    del pima
+def acquisition_plane_decision_tree2(a, t1, t2):
+    if a[5] <= t1:
+        return 0
+    else:
+        if a[0] <= t2:
+            return 2
+        else:
+            return 1
 
-    model_generation_df = model_generation_df.dropna(axis=0)
-    model_generation_df.to_excel(f"../training_outputs/{name}_model_generation_df.xlsx")
 
-    X = model_generation_df[modality_columns]
-    y = model_generation_df["Modality"]
-    return X, y
+def acquisition_plane_decision_tree(a, t1, t2):
+    if a[5] <= t1:
+        return 0
+    else:
+        if a[1] <= t2:
+            return 1
+        else:
+            return 2
 
 
-def generate_training_data2(dicom_dataframe: str, name: str):
+def generate_training_data(label_dataframe: str, dicom_dataframe: str, name: str):
     """
     Generate data for model training. Function modifies the "everything" DICOM dataframe by injecting labels from
     label_dataframe.
     :param label_dataframe: filepath to the label dataframe
     :param dicom_dataframe: filepath of "everything" dicom dataframe
     :return:
         x - training data
         y - labels
     """
-    input_output_training_columns = modality_columns + ["SeriesInstanceUID", "Modality"]
+    input_output_training_columns = plane_cols + ["Orientation", "SeriesInstanceUID"]
     input_output_training_columns = make_unique_ordered_list(
         input_output_training_columns
     )
 
-    df = pd.read_excel(dicom_dataframe)
+    label_df = pd.read_excel(label_dataframe)
+    dicom_df = pd.read_excel(dicom_dataframe)
+
+    df = pd.merge(dicom_df, label_df, on="SeriesInstanceUID")
     pima = pd.DataFrame(df[input_output_training_columns])
 
-    pima = pima[
-        (pima["Modality"] == "adc")
-        | (pima["Modality"] == "fa")
-        | (pima["Modality"] == "tracew")
-        | (pima["Modality"] == "t2w")
-        | (pima["Modality"] == "t2starw")
-        | (pima["Modality"] == "t1w")
-        | (pima["Modality"] == "flair")
-        | (pima["Modality"] == "field_map")
-        | (pima["Modality"] == "dwig")
-        | (pima["Modality"] == "dwi_multishell")
-        | (pima["Modality"] == "fmri")
-    ]
-
-    pima["Modality"].replace(imagetype_to_integer_mapping, inplace=True)
-    pima["Modality"] = pima["Modality"].astype(int)
-    pima["Modality"] = pima["Modality"].astype("category")
+    pima["Orientation"].replace(plane_to_integer_mapping, inplace=True)
+    pima["Orientation"] = pima["Orientation"].astype(int)
+    pima["Orientation"] = pima["Orientation"].astype("category")
 
     model_generation_df = pd.DataFrame(pima[input_output_training_columns])
     del pima
 
     model_generation_df = model_generation_df.dropna(axis=0)
-    model_generation_df.to_excel(f"../training_outputs/{name}_model_generation_df.xlsx")
+    model_generation_df.to_excel(
+        f"../training_outputs/{name}_model_generation_df_plane.xlsx"
+    )
 
-    X = model_generation_df[modality_columns]
-    y = model_generation_df["Modality"]
+    X = model_generation_df[plane_cols]
+    y = model_generation_df["Orientation"]
     return X, y
 
 
-# def train_model(x1, x2, x3, y1, y2, y3, use_dt):
-def train_model(use_dt):
+def train_model(x1, x2, y1, y2, use_dt):
     """
     Function to train modality classification model. By default uses Random Forrest classifier unless user specifies
     the use of Decision Tree classifier. This function also produces figures to analyze trained model and saves
     the model using skl2onnx library.
     :param x: train data
     :param y: labels
     :param use_dt: if true use Decision Tree over Random Forrest
     """
 
-    # # split data into 70% training and 30% test
-    # x1_train, x1_test, y1_train, y1_test = train_test_split(
-    #     x1, y1, test_size=0.3, random_state=1
-    # )
-    # x2_train, x2_test, y2_train, y2_test = train_test_split(
-    #     x2, y2, test_size=0.3, random_state=1
-    # )
-    # x3_train, x3_test, y3_train, y3_test = train_test_split(
-    #     x3, y3, test_size=0.3, random_state=1
-    # )
-    # x_train = pd.concat([x1_train, x2_train, x3_train], axis=0)
-    # y_train = pd.concat([y1_train, y2_train, y3_train], axis=0)
-    # x_test = pd.concat([x1_test, x2_test, x3_test], axis=0)
-    # y_test = pd.concat([y1_test, y2_test, y3_test], axis=0)
-    # print(f"SHAPE train: {y_train.shape}")
-    # print(f"SHAPE test: {y_test.shape}")
-
-    unique_df = pd.read_excel(
-        "../training_outputs/all_model_generation_df_normalized_unique.xlsx"
-    )
-    norm_df = pd.read_excel(
-        "../training_outputs/all_model_generation_df_normalized.xlsx"
-    )
-    all_df = pd.read_excel("../training_outputs/all_model_generation_df.xlsx")
-
-    uX = unique_df[modality_columns].values
-    uy = unique_df["Modality"].values
-
-    allX = all_df[modality_columns].values
-    ally = all_df["Modality"].values
-
-    # kf = KFold(n_splits=4, random_state=20, shuffle=True)
-    kf = KFold(n_splits=4, random_state=5, shuffle=True)
-
-    ti = None
-    tt = None
-    for unique_train_index, unique_test_index in kf.split(uX):
-        ti = unique_train_index
-        tt = unique_test_index
-        break
-    uX_train, uX_test = uX[ti], uX[tt]
-
-    train_indexes = []
-    test_indexes = []
-    for index, row in norm_df.iterrows():
-        if any((uX_train[:] == row[modality_columns].values).all(1)):
-            # if row[modality_columns].values in uX_train:
-            train_indexes.append(index)
-        else:
-            test_indexes.append(index)
-
-    x_train, x_test = allX[train_indexes], allX[test_indexes]
-    y_train, y_test = ally[train_indexes], ally[test_indexes]
-    print(np.unique(y_train, return_counts=True))
-    print(np.unique(y_test, return_counts=True))
-
-    # x_fi = []
-    # y_fi = []
-    # for i in range(11):
-    #     yi = np.where(y_test == i)[0][:8]
-    #     x_fi.append(x_test[yi])
-    #     y_fi.append(y_test[yi])
-    #
-    # # print(x_fi)
-    # x_test = np.array(x_fi).reshape(11*8, 11)
-    # y_test = np.array(y_fi).flatten()
-
-    # TODO: Experiment with test set of same number of examples per modality to get better Feature importance
+    # split data into 70% training and 30% test
+    x1_train, x1_test, y1_train, y1_test = train_test_split(
+        x1, y1, test_size=0.3, random_state=3
+    )
+    x2_train, x2_test, y2_train, y2_test = train_test_split(
+        x2, y2, test_size=0.3, random_state=3
+    )
+    x_train = pd.concat([x1_train, x2_train], axis=0)
+    y_train = pd.concat([y1_train, y2_train], axis=0)
+    x_test = pd.concat([x1_test, x2_test], axis=0)
+    y_test = pd.concat([y1_test, y2_test], axis=0)
 
     if use_dt:
         print("Using Decision Tree Classifier")
-        clf = DecisionTreeClassifier(max_depth=5)
+        clf = DecisionTreeClassifier(max_depth=2)
     else:
         print("Using Random Forest Classifier")
-        clf = RandomForestClassifier(n_estimators=100, max_depth=7, random_state=99)
-        # clf = AdaBoostClassifier(n_estimators=100, random_state=99, learning_rate=0.2)
+        clf = RandomForestClassifier(n_estimators=100, max_depth=3, random_state=99)
     # Train Decision Tree Classifer
     clf = clf.fit(x_train, y_train)
-    # import graphviz
-    # for i in range(3):
-    #     tree = clf.estimators_[i]
-    #     dot_data = export_graphviz(tree,
-    #                                feature_names=modality_columns,
-    #                                filled=True,
-    #                                max_depth=7,
-    #                                impurity=False,
-    #                                proportion=True)
-    #     # graph = pydotplus.graph_from_dot_data(dot_data.getvalue())
-    #     # graph.write_png(f"../training_outputs/rf_estimator_{i}.png")
-    #     graph = graphviz.Source(dot_data, format="png")
-    #     graph.render(filename=f"../training_outputs/rf_estimator_{i}")
 
     # Predict the response for test dataset
     y_pred = clf.predict(x_test)
-    print("Accuracy:", metrics.accuracy_score(y_test, y_pred))
+    y_pred_replicate = np.apply_along_axis(
+        acquisition_plane_decision_tree2, 1, x_test.values, t1=0.56, t2=0.85
+    )
+    y_pred_05_0707 = np.apply_along_axis(
+        acquisition_plane_decision_tree2, 1, x_test.values, 0.5, 0.707
+    )
+    y_pred_05_05 = np.apply_along_axis(
+        acquisition_plane_decision_tree2, 1, x_test.values, 0.5, 0.5
+    )
+    y_pred_05_085 = np.apply_along_axis(
+        acquisition_plane_decision_tree2, 1, x_test.values, 0.5, 0.85
+    )
+    y_pred_056_0707 = np.apply_along_axis(
+        acquisition_plane_decision_tree2, 1, x_test.values, 0.56, 0.707
+    )
+    y_pred_056_044 = np.apply_along_axis(
+        acquisition_plane_decision_tree, 1, x_test.values, 0.56, 0.44
+    )
+    y_pred_056_05 = np.apply_along_axis(
+        acquisition_plane_decision_tree, 1, x_test.values, 0.56, 0.5
+    )
+    y_pred_05_052 = np.apply_along_axis(
+        acquisition_plane_decision_tree, 1, x_test.values, 0.5, 0.5
+    )
+    print("Accuracy Decision Tree:", metrics.accuracy_score(y_test, y_pred))
+    print(
+        "Accuracy with thresholds of 0.56 and 0.85 (replicating the Decision Tree):",
+        metrics.accuracy_score(y_test, y_pred_replicate),
+    )
+    print(
+        "Accuracy with thresholds of 0.5 and 0.707:",
+        metrics.accuracy_score(y_test, y_pred_05_0707),
+    )
+    print(
+        "Accuracy with thresholds of 0.5 and 0.5:",
+        metrics.accuracy_score(y_test, y_pred_05_05),
+    )
+    print(
+        "Accuracy with thresholds of 0.5 and 0.85:",
+        metrics.accuracy_score(y_test, y_pred_05_085),
+    )
+    print(
+        "Accuracy with thresholds of 0.56 and 0.707:",
+        metrics.accuracy_score(y_test, y_pred_056_0707),
+    )
+    print("other tree")
+    print(
+        "Accuracy with thresholds of 0.56 and 0.44:",
+        metrics.accuracy_score(y_test, y_pred_056_044),
+    )
+    print(
+        "Accuracy with thresholds of 0.56 and 0.5:",
+        metrics.accuracy_score(y_test, y_pred_056_05),
+    )
+    print(
+        "Accuracy with thresholds of 0.5 and 0.5:",
+        metrics.accuracy_score(y_test, y_pred_05_052),
+    )
+
+    # get class report
+    rf_d = classification_report(
+        y_test,
+        y_pred,
+        target_names=list(plane_to_integer_mapping.keys()),
+        output_dict=True,
+        zero_division=True,
+    )
+    rf_df = pd.DataFrame(rf_d).transpose()
+    rf_dfs = [rf_df]
+
+    # Genereta Classification Reports and save them as CSV files
+    rf_df = pd.concat(rf_dfs, axis=0)
+    rf_df.to_excel("../training_outputs/orientation_class_report.xlsx")
 
     # Generate figures to analyze the trained model
     # https://scikit-learn.org/stable/auto_examples/text/plot_document_classification_20newsgroups.html#sphx-glr-auto-examples-text-plot-document-classification-20newsgroups-py
     fig, ax = plt.subplots(figsize=(10, 5))
     ConfusionMatrixDisplay.from_predictions(y_test, y_pred, ax=ax)
-    ax.xaxis.set_ticklabels(c)
-    ax.yaxis.set_ticklabels(c)
-    # _ = ax.set_title(
-    #     f"Confusion Matrix for {clf.__class__.__name__}\non the test data"
-    # )
-    ax.tick_params(axis="x", colors="red")
-    plt.xticks(rotation=90)
-    plt.savefig("../training_outputs/confusion_matrix.png", dpi=400)
+    ax.xaxis.set_ticklabels(plane_to_integer_mapping.keys())
+    ax.yaxis.set_ticklabels(plane_to_integer_mapping.keys())
+    _ = ax.set_title(
+        f"Confusion Matrix for {clf.__class__.__name__}\non the original data"
+    )
+    plt.savefig("../training_outputs/confusion_matrix_plane.png")
 
-    input_vector_size: int = len(modality_columns)
+    input_vector_size: int = len(plane_cols)
 
     if use_dt:
         dot_data = StringIO()
         export_graphviz(
             clf,
             out_file=dot_data,
             filled=True,
             rounded=True,
             special_characters=True,
-            feature_names=modality_columns,
-            class_names=[x for x in imagetype_to_integer_mapping.keys()],
+            feature_names=plane_cols,
+            class_names=[x for x in plane_to_integer_mapping.keys()],
         )
         graph = pydotplus.graph_from_dot_data(dot_data.getvalue())
-        graph.write_png("../training_outputs/test.png")
+        graph.write_png("../training_outputs/test_plane.png")
         # Image(graph.create_png())
-    else:
-        start_time = time.time()
-        importances = clf.feature_importances_
-        std = np.std([tree.feature_importances_ for tree in clf.estimators_], axis=0)
-        elapsed_time = time.time() - start_time
-
-        print(f"Elapsed time to compute the importances: {elapsed_time:.3f} seconds")
-
-        feature_names = modality_columns
-        forest_importances = pd.Series(importances, index=feature_names)
-
-        fig, ax = plt.subplots()
-        forest_importances.plot.bar(yerr=std, ax=ax)
-        ax.set_title("Feature importances using MDI")
-        ax.set_ylabel("Mean decrease in impurity")
-        fig.tight_layout()
-        plt.savefig("../training_outputs/rf_importance_norm.pdf")
 
     # save the model file
-    model_filename: str = "../models/rf_classifier.onnx"
+    model_filename: str = "../training_outputs/dt_classifier_plane.onnx"
     # Convert into ONNX format
     initial_type = [("float_input", FloatTensorType([None, input_vector_size]))]
     onx = convert_sklearn(
         clf, name="RandomForestImageTypeClassifier", initial_types=initial_type
     )
     with open(model_filename, "wb") as f:
         f.write(onx.SerializeToString())
 
 
-def inference_on_all_data(model_filename: str, model_df: str, out_file: str):
+def inference_on_all_data(model_filename: str):
     """
     This function runs inference on all data and produces figures dataframe containing class specific prediction.
     :param model_filename: filepath to the onnx model file.
     """
     print("\nInference on all.\n")
 
-    df = pd.read_excel(model_df)
-    e_inputs = pd.DataFrame(df[modality_columns])
+    df = pd.read_excel("../training_outputs/model_generation_df_plane.xlsx")
+    e_inputs = pd.DataFrame(df[plane_cols])
     e_inputs.fillna(-1000000, inplace=True)
     e_inputs.replace(np.nan, -1000000, inplace=True)
     e_inputs.replace("nan", -1000000, inplace=True)
 
     sess = rt.InferenceSession(model_filename)
     input_name = sess.get_inputs()[0].name
     label_name = sess.get_outputs()[0].name
@@ -336,58 +268,58 @@
     probability_onx = pred_onx_run_output[1]
     prob_df = pd.DataFrame(probability_onx)
 
     outputs = df
     outputs["GUESS_ONNX_CODE"] = pred_onx
     for col in prob_df.columns:
         outputs[f"GUESS_ONNX_idx{col}"] = prob_df[col]
-    outputs.to_excel(out_file)
+    outputs.to_excel("../training_outputs/guess_plane.xlsx")
 
 
 if __name__ == "__main__":
     # description = "author Hans J. Johnson | Script for attempting to classify image types based on dicom header fields"
     # parser = argparse.ArgumentParser(description=description)
     # parser.add_argument(
-    #     "--label_df", metavar="file", required=False, help="Path to dataframe containing labels."
+    #     "--label_df",
+    #     metavar="file",
+    #     required=False,
+    #     help="Path to dataframe containing labels.",
     # )
     # parser.add_argument(
-    #     "--dicom_df", metavar="file", required=False, help="Output path for Dicom Dataframe."
+    #     "--dicom_df",
+    #     metavar="file",
+    #     required=False,
+    #     help="Output path for Dicom Dataframe.",
     # )
     # parser.add_argument(
-    #     "--use_DT", action="store_true", required=False, help="Ruleset defining config file."
+    #     "--use_DT",
+    #     action="store_true",
+    #     required=False,
+    #     help="Use decision tree over Random Forest.",
     # )
-    #
+
     # if len(sys.argv) == 1:
     #     parser.print_help()
     #     exit(1)
     # args = parser.parse_args()
 
     # data
-    # i_dcmf_df = "../data/iowaStroke_all_dicom.xlsx"
-    # i_lbl_df = "../data/iowaStroke_labels.xlsx"
-    # ix, iy = generate_training_data(i_lbl_df, i_dcmf_df, "iowaStroke")
-
-    # p_dcmf_df = "../data/prostate_all_dicom_raw.xlsx"
-    # p_lbl_df = "../data/prostate_labels.xlsx"
-    # px, py = generate_training_data(p_lbl_df, p_dcmf_df, "prostate")
-    #
-    # t_dcmf_df = "../data/trackOn_all_dicom_raw.xlsx"
-    # tx, ty = generate_training_data2(t_dcmf_df, "trackOn")
-
-    # train_model(x1=ix, x2=px, x3=tx, y1=iy, y2=py, y3=ty, use_dt=False)
-    train_model(use_dt=False)
-
-    inference_on_all_data(
-        "../models/rf_classifier.onnx",
-        "../training_outputs/iowaStroke_model_generation_df.xlsx",
-        "../training_outputs/iowaStroke_guess.xlsx",
-    )
-    inference_on_all_data(
-        "../models/rf_classifier.onnx",
-        "../training_outputs/prostate_model_generation_df.xlsx",
-        "../training_outputs/prostate_guess.xlsx",
-    )
-    inference_on_all_data(
-        "../models/rf_classifier.onnx",
-        "../training_outputs/trackOn_model_generation_df.xlsx",
-        "../training_outputs/trackOn_guess.xlsx",
-    )
+    i_dcmf_df = "../data/iowaStroke_all_dicom.xlsx"
+    i_lbl_df = "../data/iowaStroke_labels.xlsx"
+    ix, iy = generate_training_data(i_lbl_df, i_dcmf_df, "iowaStroke")
+
+    p_dcmf_df = "../data/prostate_all_dicom_raw.xlsx"
+    p_lbl_df = "../data/prostate_labels.xlsx"
+    px, py = generate_training_data(p_lbl_df, p_dcmf_df, "prostate")
+
+    df1 = pd.read_excel("../training_outputs/iowaStroke_model_generation_df_plane.xlsx")
+    df2 = pd.read_excel("../training_outputs/prostate_model_generation_df_plane.xlsx")
+    df = pd.concat([df1, df2], axis=0, ignore_index=True)
+    print(df.shape)
+    df.to_excel("../training_outputs/model_generation_df_plane.xlsx")
+
+    train_model(ix, px, iy, py, use_dt=True)
+    inference_on_all_data("../training_outputs/dt_classifier_plane.onnx")
+
+    # TODO: add additional inference function to run inference on new data
+    # TODO: Add flags to control file creation. Example idea to create a data directory where
+    #  all dataframes will be written, similarly figure directory, and specify exact model output path, etc.
```

### Comparing `dcm_classifier-0.6.0rc9/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.7.0rc1/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/scripts/todo_list` & `dcm_classifier-0.7.0rc1/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,54 +47,54 @@
     "SliceThickness",
 ]
 
 optional_DICOM_fields: list[str] = [
     "SAR",  # Not present in all derived image types
     "ImageType",  # Not required
     "Manufacturer",  # Not required
-    "Contrast/BolusAgent",  # "(0x0018, 0x0010)"
+    "ContrastBolusAgent",  # "(0x0018, 0x0010)"
     "Diffusionb-value",  # Not required
     "Diffusionb-valueMax",  # Not required
-    "Echo Number(s)",
-    "Echo Train Length",
-    "Scanning Sequence",
-    "Sequence Variant",
-    "In-plane Phase Encoding Direction",
-    "dB/dt",
-    "Imaging Frequency",
-    "MR Acquisition Type",
-    "Number of Averages",
-    "Inversion Time",
-    "Variable Flip Angle Flag",
+    "EchoNumbers",
+    "EchoTrainLength",
+    "ScanningSequence",
+    "SequenceVariant",
+    "InPlanePhaseEncodingDirection",
+    "dBdt",
+    "ImagingFrequency",
+    "MRAcquisitionType",
+    "NumberOfAverages",
+    "InversionTime",
+    "VariableFlipAngleFlag",
     "AcquisitionTime",
 ]
 
 inference_features: list[str] = [
     "Diffusionb-valueBool",
     "EchoTime",
-    "Echo Train Length",
+    "EchoTrainLength",
     "FlipAngle",
     "HasDiffusionGradientOrientation",
-    "Image Type_ADC",
-    "Image Type_DERIVED",
-    "Image Type_DIFFUSION",
-    "Image Type_EADC",
-    "Image Type_FA",
-    "Image Type_ORIGINAL",
-    "Image Type_TRACEW",
-    "Imaging Frequency",
-    "Inversion Time",
+    "ImageType_ADC",
+    "ImageType_DERIVED",
+    "ImageType_DIFFUSION",
+    "ImageType_EADC",
+    "ImageType_FA",
+    "ImageType_ORIGINAL",
+    "ImageType_TRACEW",
+    "ImagingFrequency",
+    "InversionTime",
     "Manufacturer_siemens",
-    "Number of Averages",
+    "NumberOfAverages",
     "PixelBandwidth",
     "RepetitionTime",
     "SAR",
-    "Scanning Sequence_GR",
-    "Scanning Sequence_IR",
-    "Scanning Sequence_SE",
-    "Sequence Variant_MP",
-    "Sequence Variant_SP",
-    "dB/dt",
+    "ScanningSequence_GR",
+    "ScanningSequence_IR",
+    "ScanningSequence_SE",
+    "SequenceVariant_MP",
+    "SequenceVariant_SP",
+    "dBdt",
     "has_b0",
     "has_pos_b0",
     "likely_diffusion",
 ]
```

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,36 +31,50 @@
         volume_info_list (List[DicomSingleVolumeInfoBase]): A list to store
             DicomSingleVolumeInfoBase objects for this series.
         series_modality (Optional[str]): The modality of the series (e.g., "CT", "MRI").
         modality_probability (Optional[pd.DataFrame]): A DataFrame containing modality
             probabilities.
         acquisition_plane (Optional[str]): The acquisition plane of the series (e.g.,
             "Sagittal", "Axial").
+        is_isotropic (bool): A flag indicating whether the series is isotropic.
+        has_contrast (bool): A flag indicating whether the series has contrast.
 
     Methods:
         get_series_number(self) -> int:
 
-        set_modality(self, modality: str) -> None:
+        set_series_modality(self, modality: str) -> None:
 
-        get_modality(self) -> str:
+        get_series_modality(self) -> str:
 
         set_modality_probabilities(self, modality_probability: pd.DataFrame) -> None:
 
         get_modality_probabilities(self) -> pd.DataFrame:
 
+        set_is_isotropic(self, isotropic: bool) -> None:
+
+        get_is_isotropic(self) -> bool:
+
+        set_has_contrast(self, contrast: bool) -> None:
+
+        get_has_contrast(self) -> bool:
+
         set_acquisition_plane(self, acquisition_plane: str) -> None:
 
         get_acquisition_plane(self) -> str:
 
         get_volume_list(self) -> List[DicomSingleVolumeInfoBase]:
 
         add_volume_to_series(self, new_volume_info: DicomSingleVolumeInfoBase) -> None:
 
+        organize_volumes(self) -> None:
+
         get_series_info_dict(self) -> Dict[str, Any]:
 
+        get_series_uid(self) -> str:
+
     """
 
     def __init__(
         self,
         series_number: int,
     ) -> None:
         """
@@ -241,15 +255,18 @@
         self.organize_volumes()
 
     def organize_volumes(self) -> None:
         """
         Organize the subvolumes within the series based on acquisition time.
         """
         # AcquisitionTime is an optional field, this might need to be changed in the future
-        sorted(self.volume_info_list, key=lambda x: x.get_volume_dictionary()["AcquisitionTime"])
+        sorted(
+            self.volume_info_list,
+            key=lambda x: x.get_volume_dictionary().get("AcquisitionTime", -12345),
+        )
         # assign the index to each volume
         for index, volume in enumerate(self.volume_info_list):
             volume.set_volume_index(index)
 
     def get_series_info_dict(self) -> dict[str, Any]:
         """
         Get a dictionary with information about the series.
```

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,30 +50,51 @@
         _pydicom_info (pydicom.Dataset): A pydicom.Dataset containing information about the DICOM volume.
         bvalue (float): The b-value of the DICOM volume.
         volume_info_dict (Dict[str, Any]): A dictionary containing information about the DICOM volume.
         itk_image (Optional[FImageType]): The ITK image of the DICOM volume.
         volume_modality (Optional[str]): The modality of the DICOM volume (e.g., "CT", "MRI").
         modality_probability (Optional[pd.DataFrame]): A DataFrame containing modality probabilities.
         acquisition_plane (Optional[str]): The acquisition plane of the DICOM volume (e.g., "Sagittal", "Axial").
+        is_isotropic (Optional[bool]): True if the DICOM volume is isotropic, False otherwise.
+        has_contrast (Optional[bool]): True if the DICOM volume has contrast, False otherwise.
+        parent_series (Optional[DicomSingleSeries]): The parent series of the DICOM volume.
+        volume_index (Optional[int]): The index of the DICOM volume within its series.
+        has_diffusion_gradient (bool): True if the DICOM volume has diffusion gradient, False otherwise.
 
     Methods:
-        set_modality(self, modality: str) -> None:
+        get_volume_series_description(self) -> str:
 
-        get_modality(self) -> str:
+        set_volume_modality(self, modality: str) -> None:
+
+        get_volume_modality(self) -> str:
+
+        get_series_modality(self) -> str:
+
+        set_is_isotropic(self, isotropic: bool) -> None:
+
+        get_is_isotropic(self) -> bool:
+
+        set_has_contrast(self, contrast: bool) -> None:
+
+        get_has_contrast(self) -> bool:
+
+        get_contrast_agent(self) -> str:
+
+        set_parent_series(self, series) -> None:
+
+        get_parent_series(self):
 
         set_modality_probabilities(self, modality_probability: pd.DataFrame) -> None:
 
         get_modality_probabilities(self) -> pd.DataFrame:
 
         set_acquisition_plane(self, acquisition_plane: str) -> None:
 
         get_acquisition_plane(self) -> str:
 
-        get_volume_dictionary(self) -> Dict[str, Any]:
-
         get_primary_volume_info(self, vol_index: int = 0) -> Dict[str, str]:
 
         get_itk_image(self) -> FImageType:
 
         get_series_uid(self) -> str:
 
         get_study_uid(self) -> str:
@@ -82,25 +103,28 @@
 
         get_series_size(self) -> str:
 
         get_one_volume_dcm_filenames(self) -> List[Path]:
 
         get_volume_dictionary(self) -> Dict[str, Any]:
 
-        get_volume_datatype(self) -> str:
-
         get_volume_bvalue(self) -> float:
 
         get_series_number(self) -> int:
 
+        get_volume_index(self) -> int | None:
+
+        set_volume_index(self, volume_index: int) -> None:
+
         is_MR_modality(self):
 
         _make_one_study_info_mapping_from_filelist(self) -> (str, dict):
 
         get_image_diagnostics(self) -> str:
+
     """
 
     def __init__(self, one_volume_dcm_filenames: list[Path | str]) -> None:
         """
         Initializes a DicomSingleVolumeInfoBase instance with a list of DICOM file paths.
 
         Args:
@@ -496,19 +520,19 @@
         )
         volume_info_dict["has_b0"] = 1 if bvalue_current_dicom == 0 else 0
         volume_info_dict["has_pos_b0"] = 1 if bvalue_current_dicom > 0 else 0
         volume_info_dict["HasDiffusionGradientOrientation"] = int(
             self.has_diffusion_gradient
         )
         if (
-            volume_info_dict["Image Type_DIFFUSION"] == 1
-            or volume_info_dict["Image Type_ADC"] == 1
-            or volume_info_dict["Image Type_EADC"] == 1
-            or volume_info_dict["Image Type_TRACEW"] == 1
-            or volume_info_dict["Image Type_FA"] == 1
+            volume_info_dict["ImageType_DIFFUSION"] == 1
+            or volume_info_dict["ImageType_ADC"] == 1
+            or volume_info_dict["ImageType_EADC"] == 1
+            or volume_info_dict["ImageType_TRACEW"] == 1
+            or volume_info_dict["ImageType_FA"] == 1
             or volume_info_dict["Diffusionb-value"] > 0
             or volume_info_dict["HasDiffusionGradientOrientation"] == 1
         ):
             volume_info_dict["likely_diffusion"] = 1
         else:
             volume_info_dict["likely_diffusion"] = 0
         # those values are 1 in case of a single volume
```

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/image_type_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,24 +49,33 @@
     Inference class for image type classification. The base implementation is for our standard model. This class
     can be customized by users to implement their own models for targeted for specific datasets.
 
     Attributes:
         classification_model_filename (Union[str, Path]): Path to the classification model file (base implementation requires ONNX file).
         classification_feature_list (List[str]): List of features used for classification.
         image_type_map (Dict[str, str]): Mapping between class name and model integer output.
-        mode (str): "series" or "volume" to run inference on series or volume level (a series could have multiple subvolumes).
         min_probability_threshold (float): Minimum probability threshold for classification, defaults to 0.4. If maximum class probability is below this threshold, the image type is set to "unknown".
 
     Methods:
+        get_min_probability_threshold(self) -> float:
+
         get_int_to_type_map(self) -> dict:
 
+        _update_diffusion_series_modality(self) -> None:
+
+        check_if_diffusion(self) -> None:
+
         set_series(self, series: DicomSingleSeries) -> None:
 
         infer_acquisition_plane(self, feature_dict: dict = None) -> str:
 
+        infer_isotropic(self, feature_dict: dict = None) -> bool | None:
+
+        infer_contrast(self, feature_dict: dict = None) -> bool | None:
+
         infer_modality(self, feature_dict: dict = None) -> (str, pd.DataFrame):
 
         run_inference(self) -> None:
     """
 
     def __init__(
         self,
@@ -197,28 +206,28 @@
         # check if the volume is isotropic
         spacing = np.array(feature_dict["PixelSpacing"])
         thickness = float(feature_dict["SliceThickness"])
         if np.allclose(spacing, thickness, rtol=0.1):
             return True
         return False
 
-    def infer_contrast(self, feature_dict: dict = None) -> bool | None:
+    def infer_contrast(self, feature_dict: dict = None) -> bool:
         """
         Infer whether the image has contrast based on DICOM information and image properties.
         Args:
             feature_dict: A dictionary containing features used for classification.
 
         Returns:
             bool: True if the image has contrast, False otherwise.
         """
         # check if the volume was invalidated
 
-        field = "Contrast/BolusAgent"
+        field = "ContrastBolusAgent"
         if field not in feature_dict.keys():
-            return None
+            return False
 
         # check if the volume has contrast
         if "none" not in feature_dict[field].lower():
             return True
         return False
 
     def infer_modality(self, feature_dict: dict = None) -> (str, pd.DataFrame):
@@ -299,27 +308,19 @@
 
     def run_inference(self):
         """
         Run image type inference for the specified DICOM series or volumes.
 
         This method performs image type classification and acquisition plane inference based on the provided features.
 
-        If the `mode` is set to "series," inference is performed on the entire series, and modality and acquisition
-        plane information is updated for the series.
-
-        If the `mode` is set to "volume," inference is performed for each volume within the series, and modality and
-        acquisition plane information is updated for each volume.
-
         Args:
             None
 
         Returns:
             None
-        Raises:
-            ValueError: If an unsupported `mode` is specified.
         """
 
         def validate_features(input_dict: dict) -> bool:
             """
             Validate the presence of required features in the input feature dictionary.
 
             This function checks if all the features specified in the `classification_feature_list` are present in
@@ -413,14 +414,15 @@
             else:
                 if "pd" in unique_modalities and "t2w" in unique_modalities:
                     self.series.set_series_modality("PDT2")
                 # DWI series usually contains b0 and dwig gradient volumes
                 elif "dwig" in unique_modalities:
                     self._update_diffusion_series_modality()
                 # TRACEW series often contains b0 and tracew volumes
+                # TODO: get more data for testing
                 elif "tracew" in unique_modalities:
                     self.series.set_series_modality("tracew")
                 elif -12345 not in unique_bvals:
                     self._update_diffusion_series_modality()
                 else:
                     # if other scenarios are not met, we set the modality to the first volume's modality
                     self.series.set_series_modality(
```

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/study_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         validate(self):
 
         __identify_single_volumes(
             self,
             study_directory: Path,
         ) -> Dict[int, DicomSingleSeries]:
 
-        series_inference(self):
     """
 
     series_restrictions_list_dwi_subvolumes: list[str] = [
         # https://www.na-mic.org/wiki/NAMIC_Wiki:DTI:DICOM_for_DWI_and_DTI
         # STANDARD
         "0018|9075",  # S 1 Diffusion Directionality
         "0018|9076",  # SQ 1 Diffusion Gradient Direction Sequence
```

### Comparing `dcm_classifier-0.6.0rc9/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.7.0rc1/src/dcm_classifier/utility_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -162,30 +162,39 @@
         }
     )
     # TODO: https://pydicom.github.io/pydicom/dev/auto_examples/metadata_processing/plot_add_dict_entries.html
     # Add these private tags to the DICOM dictionary for better processing
 
     for k, v in private_tags_map.items():
         if v in dicom_header_info:
+            # ensure safe extraction of the dicom element
+            if isinstance(dicom_header_info[v], pydicom.dataelem.RawDataElement):
+                dicom_element = pydicom.dataelem.DataElement_from_raw(
+                    dicom_header_info[v]
+                )
+            else:
+                dicom_element = dicom_header_info[v]
+
             # This decoding of bvalues follows the NAMIC conventions defined at
             # https://www.na-mic.org/wiki/NAMIC_Wiki:DTI:DICOM_for_DWI_and_DTI
-            dicom_element = dicom_header_info[v]
+            # TODO: add testing for this
             if v == private_tags_map["GE"]:
                 large_number_modulo_for_GE = 100000
                 # value = dicom_element.value[0] % large_number_modulo_for_GE
                 # TODO: This is a hack to get around an error. Might be due to missing data in SickKids project
                 try:
                     value = dicom_element.value[0] % large_number_modulo_for_GE
                 except TypeError:
                     return -12345
             elif v == private_tags_map["Siemens_historical"]:
                 # This is not supported yet
                 continue
             else:
                 value = dicom_element.value
+            # TODO: add testing for this
             if dicom_element.VR == "OB":
                 if isinstance(value, bytes):
                     value = value.decode("utf-8", "backslashreplace")
                 elif isinstance(value, numbers.Number):
                     pass
                 else:
                     print(
@@ -204,15 +213,15 @@
                 return -12345
             if round_to_nearst_10:
                 result = round(result / 10.0) * 10
             return result
     return -12345
 
 
-def test_magnitude_of_1(vector: np.ndarray) -> bool:
+def ensure_magnitude_of_1(vector: np.ndarray) -> bool:
     """
     Ensure that the magnitude of a vector is 1.
 
     Args:
         vector (np.ndarray): The input vector.
 
     Returns:
@@ -246,15 +255,21 @@
             "UHI": (0x0065, 0x1037),
             # "Toshiba" : # Uses (0x0018, 0x9087) standard
         }
     )
     gradient_direction = None
     for k, v in private_tags_map.items():
         if v in dicom_header_info:
-            gradient_direction_element = dicom_header_info[v]
+            # ensure safe extraction of the dicom element
+            if isinstance(dicom_header_info[v], pydicom.dataelem.RawDataElement):
+                gradient_direction_element = pydicom.dataelem.DataElement_from_raw(
+                    dicom_header_info[v]
+                )
+            else:
+                gradient_direction_element = dicom_header_info[v]
             if v == private_tags_map["Siemens"]:
                 gradient_direction_raw = gradient_direction_element.value
                 if (
                     gradient_direction_element.VR == "OB"
                     and len(gradient_direction_raw) == 24
                 ):
                     gradient_direction = np.frombuffer(
@@ -270,15 +285,17 @@
                     break
                 except TypeError:
                     gradient_direction = None
 
     # ensure that the gradient direction is a 3D vector
     if gradient_direction is not None:
         gradient_direction_size = gradient_direction.size
-        if gradient_direction_size != 3 or not test_magnitude_of_1(gradient_direction):
+        if gradient_direction_size != 3 or not ensure_magnitude_of_1(
+            gradient_direction
+        ):
             gradient_direction = None
 
     return gradient_direction
 
 
 def infer_diffusion_from_gradient(filenames: list[Path]) -> str:
     """
@@ -328,257 +345,281 @@
     ro_dataset: pydicom.Dataset,
     required_info_list: list[str],
     optional_info_list: list[str],
 ) -> tuple[dict, bool]:
     """
     Validates the DICOM fields in the DICOM header to ensure all required fields are present.
 
-    Raises an exception if any required fields are missing.
+    Args:
+        ro_dataset (pydicom.Dataset): The input DICOM dataset.
+        required_info_list (list[str]): A list of required DICOM fields.
+        optional_info_list (list[str]): A list of optional DICOM fields.
 
+    Returns:
+        tuple[dict, bool]: A dictionary containing the sanitized DICOM fields and a boolean indicating whether the validation was successful.
+
+    Raises an exception if any required fields are missing.
     """
     dataset_dictionary: dict[str, Any] = dict()
     dataset = deepcopy(ro_dataset)  # DO NOT MODIFY THE INPUT DATASET!
     dicom_filename: Path = dataset.filename
     dataset_dictionary["FileName"]: str = dicom_filename
     dataset = pydicom.Dataset(dataset)  # DO NOT MODIFY THE INPUT DATASET!
     dataset.remove_private_tags()
-    values = dataset.values()
     INVALID_VALUE = "INVALID_VALUE"
-    all_candidate_info_fields: list[str] = required_info_list + optional_info_list
-
-    for v in values:
-        if isinstance(v, pydicom.dataelem.RawDataElement):
-            e = pydicom.dataelem.DataElement_from_raw(v)
-        else:
-            e = v
-
-        # process the name to match naming in required_info_list
-        name = str(e.name).replace(" ", "").replace("(", "").replace(")", "")
-        # Only add entities that are in the required or optional lists
-
-        if name in all_candidate_info_fields:
-            value = e.value
-            dataset_dictionary[name] = value
-
-    del all_candidate_info_fields
 
     # check if all fields in the required_info_list are present in dataset dictionary.
     # If fields are not present, or they are formatted incorrectly, add them with INVALID_VALUE
     missing_fields = []
     for field in required_info_list:
-        if field not in dataset_dictionary.keys():
+        if field not in dataset:
             # RepetitionTime and EchoTime might not be present in ADC images.
             # Therefore, if they are missing, set them to -12345
             if field == "RepetitionTime" or field == "EchoTime":
                 dataset_dictionary[field] = -12345
             else:
                 dataset_dictionary[field] = INVALID_VALUE
                 missing_fields.append(field)
         elif field == "EchoTime" or field == "RepetitionTime":
-            if (
-                dataset_dictionary[field] is None
-                or str(dataset_dictionary[field]) == ""
-            ):
+            if dataset[field].value is None or str(dataset[field].value) == "":
                 # ADC sequences may not have EchoTime
                 dataset_dictionary[field] = -12345
-            elif not is_number(dataset_dictionary[field]):
+            elif not is_number(dataset[field].value):
                 dataset_dictionary[field] = INVALID_VALUE
                 missing_fields.append(field)
                 vprint(f"Missing required {field} value {dicom_filename}")
+            else:
+                dataset_dictionary[field] = dataset[field].value
         elif field == "SeriesNumber":
-            if not is_integer(dataset_dictionary[field]):
+            if not is_integer(dataset[field].value):
                 dataset_dictionary[field] = INVALID_VALUE
                 missing_fields.append(field)
                 vprint(f"Missing required {field} value {dicom_filename}")
+            else:
+                dataset_dictionary[field] = dataset[field].value
         elif field == "PixelBandwidth":
-            if not is_number(dataset_dictionary[field]):
+            if not is_number(dataset[field].value):
                 dataset_dictionary[field] = INVALID_VALUE
                 missing_fields.append(field)
                 vprint(f"Missing required {field} value {dicom_filename}")
+            else:
+                dataset_dictionary[field] = dataset[field].value
         elif field == "SliceThickness":
-            if not is_number(dataset_dictionary[field]):
+            if not is_number(dataset[field].value):
                 dataset_dictionary[field] = INVALID_VALUE
                 missing_fields.append(field)
                 vprint(f"Missing required {field} value {dicom_filename}")
+            else:
+                dataset_dictionary[field] = dataset[field].value
         elif field == "PixelSpacing":
             try:
-                dataset_dictionary[field] = np.array(dataset_dictionary[field])
+                dataset_dictionary[field] = np.array(dataset[field].value)
             except Exception as e:
                 dataset_dictionary[field] = INVALID_VALUE
                 missing_fields.append(field)
                 vprint(f"Missing required {field} value {dicom_filename}:\n{e}")
         else:
             # check that the field is not empty or None
-            if (
-                dataset_dictionary[field] is None
-                or str(dataset_dictionary[field]) == ""
-            ):
+            if dataset[field].value is None or str(dataset[field].value) == "":
                 dataset_dictionary[field] = INVALID_VALUE
                 missing_fields.append(field)
                 vprint(f"Missing required field {dicom_filename}")
+            else:
+                dataset_dictionary[field] = dataset[field].value
 
     # set the default values for optional dicom fields
     for field in optional_info_list:
         if field == "SAR":
-            if field not in dataset_dictionary.keys() or not is_number(
-                dataset_dictionary[field]
-            ):
+            if field not in dataset or not is_number(dataset[field].value):
                 # SAR is allowed to be empty or not a number because derived images often do not have SAR
                 # for example, ADC images are derived images that are computed, so there is not
                 # SAR impact on the patient for the derived image.
                 # SAR Calculated whole body Specific Absorption Rate in watts/kilogram.
                 # indicate that there is no SAR for the computed image
                 _default_inferred_value = -12345.0
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
+            else:
+                dataset_dictionary[field] = dataset[field].value
         elif field == "Manufacturer":
-            if field not in dataset_dictionary.keys():
+            if field not in dataset:
                 # Manufacturer is not a required field, it can be unknown
                 _default_inferred_value = "UnknownManufacturer"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
+            else:
+                dataset_dictionary[field] = dataset[field].value
         elif field == "ImageType":
-            if field not in dataset_dictionary.keys():
+            if field not in dataset:
                 # ImageType is not a required field, it can be unknown
                 _default_inferred_value = "UnknownImageType"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Contrast/BolusAgent":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "ContrastBolusAgent":
+            if field not in dataset:
                 # if (
                 #     dataset_dictionary[field] is None
                 #     or str(dataset_dictionary[field]) == ""
                 # ):
                 # The contrast is required but is empty if unknown but also may not be in every dataset
                 dataset_dictionary[field] = "None"
-        elif field == "Echo Number(s)":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "EchoNumbers":
+            if field not in dataset:
                 # EchoNumber(s) is not a required field, it can be unknown
                 _default_inferred_value = -12345
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Echo Train Length":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "EchoTrainLength":
+            if field not in dataset:
                 # EchoTrainLength is not a required field, it can be unknown
                 _default_inferred_value = -12345
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Scanning Sequence":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "ScanningSequence":
+            if field not in dataset:
                 # ScanningSequence is not a required field, it can be unknown
                 _default_inferred_value = "UnknownScanningSequence"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Sequence Variant":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "SequenceVariant":
+            if field not in dataset:
                 # SequenceVariant is not a required field, it can be unknown
                 _default_inferred_value = "UnknownSequenceVariant"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "In-plane Phase Encoding Direction":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "InPlanePhaseEncodingDirection":
+            if field not in dataset:
                 # InplanePhaseEncodingDirection is not a required field, it can be unknown
                 _default_inferred_value = "UnknownInplanePhaseEncodingDirection"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "dB/dt":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "dBdt":
+            if field not in dataset:
                 # dBdt is not a required field, it can be unknown
                 _default_inferred_value = -12345
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Imaging Frequency":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "ImagingFrequency":
+            if field not in dataset:
                 # ImagingFrequency is not a required field, it can be unknown
                 _default_inferred_value = -12345
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "MR Acquisition Type":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "MRAcquisitionType":
+            if field not in dataset:
                 # MRAcquisitionType is not a required field, it can be unknown
                 _default_inferred_value = "UnknownMRAcquisitionType"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Number of Averages":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "NumberOfAverages":
+            if field not in dataset:
                 # NumberOfAverages is not a required field, it can be unknown
                 _default_inferred_value = -12345
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Inversion Time":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "InversionTime":
+            if field not in dataset:
                 # InversionTime is not a required field, it can be unknown
                 _default_inferred_value = -12345
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
-        elif field == "Variable Flip Angle Flag":
-            if field not in dataset_dictionary.keys():
+            else:
+                dataset_dictionary[field] = dataset[field].value
+        elif field == "VariableFlipAngleFlag":
+            if field not in dataset:
                 # VariableFlipAngleFlag is not a required field, it can be unknown
                 _default_inferred_value = "UnknownVariableFlipAngleFlag"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
+            else:
+                dataset_dictionary[field] = dataset[field].value
         elif field == "AcquisitionTime":
-            if field not in dataset_dictionary.keys():
-                # InversionTime is not a required field, it can be unknown
+            if field not in dataset:
+                # AcquisitionTime is not a required field, it can be unknown
                 _default_inferred_value = -12345
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
+            else:
+                dataset_dictionary[field] = dataset[field].value
 
     # Warn the user if there are INVALID_VALUE fields
     if len(missing_fields) > 0:
+        print(f"\n\n\n{missing_fields}\n\n\n")
         warnings.warn(
             f"\nWARNING: Required DICOM fields: {missing_fields} in {dicom_filename} are missing or have invalid values.\n"
         )
         return dataset_dictionary, False
 
     return dataset_dictionary, True
 
 
 # organize required features
 image_type_features: list[str] = [
-    field for field in features if ("Image Type_" in field and "ADC" not in field)
+    field for field in features if ("ImageType_" in field and "ADC" not in field)
 ]
 manufacturer_features: list[str] = [
     field for field in features if "Manufacturer_" in field
 ]
 scanning_sequence_features: list[str] = [
-    field for field in features if "Scanning Sequence_" in field
+    field for field in features if "ScanningSequence_" in field
 ]
 scanning_variant_features: list[str] = [
-    field for field in features if "Sequence Variant_" in field
+    field for field in features if "SequenceVariant_" in field
 ]
 
 
 def get_coded_dictionary_elements(
     dicom_sanitized_dataset: dict,
 ) -> dict[str, Any]:
     """
@@ -601,24 +642,24 @@
             # Return a completely empty dictionary if any required values are missing from image
             # This should likely be more robust in the future
             return dict()
         elif name == "ImageType":
             lower_value_str: str = str(value).lower()
             if "adc" in lower_value_str:
                 if "eadc" in lower_value_str:
-                    dataset_dictionary["Image Type_EADC"] = 1
-                    dataset_dictionary["Image Type_ADC"] = 0
+                    dataset_dictionary["ImageType_EADC"] = 1
+                    dataset_dictionary["ImageType_ADC"] = 0
                 else:
-                    dataset_dictionary["Image Type_ADC"] = 1
-                    dataset_dictionary["Image Type_EADC"] = 0
+                    dataset_dictionary["ImageType_ADC"] = 1
+                    dataset_dictionary["ImageType_EADC"] = 0
             else:
-                dataset_dictionary["Image Type_ADC"] = 0
-                dataset_dictionary["Image Type_EADC"] = 0
+                dataset_dictionary["ImageType_ADC"] = 0
+                dataset_dictionary["ImageType_EADC"] = 0
 
-            throw_away: int = len("Image Type_")
+            throw_away: int = len("ImageType_")
             for feature in image_type_features:
                 if feature[throw_away:].lower() in lower_value_str:
                     dataset_dictionary[feature] = 1
                 else:
                     dataset_dictionary[feature] = 0
         elif name == "ImageOrientationPatient":
             tuple_list = convert_array_to_index_value(name, value)
@@ -628,39 +669,39 @@
             lower_manufacturer_string: str = str(value).lower()
             throw_away: int = len("Manufacturer_")
             for feature in manufacturer_features:
                 if feature[throw_away:].lower() in lower_manufacturer_string:
                     dataset_dictionary[feature] = 1
                 else:
                     dataset_dictionary[feature] = 0
-        elif name == "Scanning Sequence":
+        elif name == "ScanningSequence":
             lower_scanning_sequence_string: str = str(value).lower()
-            throw_away: int = len("Scanning Sequence_")
+            throw_away: int = len("ScanningSequence_")
             for feature in scanning_sequence_features:
                 if feature[throw_away:].lower() in lower_scanning_sequence_string:
                     dataset_dictionary[feature] = 1
                 else:
                     dataset_dictionary[feature] = 0
-        elif name == "Sequence Variant":
+        elif name == "SequenceVariant":
             lower_sequence_variant_string: str = str(value).lower()
-            throw_away: int = len("Sequence Variant_")
+            throw_away: int = len("SequenceVariant_")
             for feature in scanning_variant_features:
                 if feature[throw_away:].lower() in lower_sequence_variant_string:
                     dataset_dictionary[feature] = 1
                 else:
                     dataset_dictionary[feature] = 0
-        elif name == "Contrast/BolusAgent":
+        elif name == "ContrastBolusAgent":
             no_contrast_list = ["none", "no", "no contrast", "no_contrast", "n"]
             if str(value).lower() in no_contrast_list:
-                dataset_dictionary["Contrast/BolusAgent"] = "None"
+                dataset_dictionary["ContrastBolusAgent"] = "None"
             else:
                 try:
-                    dataset_dictionary["Contrast/BolusAgent"] = str(value)
+                    dataset_dictionary["ContrastBolusAgent"] = str(value)
                 except TypeError:
-                    dataset_dictionary["Contrast/BolusAgent"] = "INVALID_VALUE"
+                    dataset_dictionary["ContrastBolusAgent"] = "INVALID_VALUE"
 
         else:
             dataset_dictionary[name] = str(value)
 
     return dataset_dictionary
```

### Comparing `dcm_classifier-0.6.0rc9/tests/conftest.py` & `dcm_classifier-0.7.0rc1/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,22 +63,39 @@
     study.series_dictionary.get(13),
     study.series_dictionary.get(14),
     study.series_dictionary.get(15),
 ]
 flair_series = [study.series_dictionary.get(7)]
 t2_series = [study.series_dictionary.get(11)]
 adc_series = [study.series_dictionary.get(6)]
+tracew_series = [study.series_dictionary.get(5)]
+
+
+dwi_study = ProcessOneDicomStudyToVolumesMappingBase(
+    study_directory=(testing_dicom_dir / "anonymized_dwi_series"), inferer=inferer
+)
+dwi_study.run_inference()
+
+
+@pytest.fixture(scope="session")
+def get_dwi_study():
+    return dwi_study
 
 
 @pytest.fixture(scope="session")
 def get_data_dir():
     return testing_dicom_dir / "anonymized_data"
 
 
 @pytest.fixture(scope="session")
+def mock_tracew_series():
+    return tracew_series
+
+
+@pytest.fixture(scope="session")
 def mock_ax_series():
     return ax_series
 
 
 @pytest.fixture(scope="session")
 def mock_sag_series():
     return sag_series
```

### Comparing `dcm_classifier-0.6.0rc9/tests/testing_data/anonymized_testing_data.tar.gz` & `dcm_classifier-0.7.0rc1/tests/testing_data/anonymized_testing_data.tar.gz`

 * *Files 20% similar despite different names*

#### anonymized_testing_data.tar

##### file list

```diff
@@ -1,502 +1,533 @@
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-12-06 19:05:54.000000 anonymized_testing_data/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/5/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149132 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149148 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149134 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2023-11-15 19:46:38.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149134 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111492 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64880 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:39.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64880 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234544 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234538 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234548 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234540 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234538 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832592 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832592 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832602 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832592 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/15/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   653408 2023-11-15 19:46:40.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653402 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653406 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653410 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653408 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653408 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653406 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653404 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653402 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653410 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653398 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653398 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653404 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653402 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/3/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/3/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    66394 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66382 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66384 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218166 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111704 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111694 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111694 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111696 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111700 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166946 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166948 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166956 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166952 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:41.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111492 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314412 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314412 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314410 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314416 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314412 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314410 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   149114 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149110 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149110 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149116 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149116 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149116 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149114 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/2/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/2/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    66392 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66388 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66390 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66390 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66390 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/4/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/4/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    66396 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66394 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66382 2023-11-15 19:46:42.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)       45 2023-12-06 19:05:54.000000 anonymized_testing_data/anonymized_testing_data.tar.gz
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 22:31:16.000000 anonymized_testing_data/invalid_data/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 22:27:25.000000 anonymized_testing_data/invalid_data/invalid_fields/
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2023-11-15 22:27:24.000000 anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2023-11-15 22:27:24.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2023-11-15 22:27:25.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2023-11-15 22:27:25.000000 anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64842 2023-11-15 22:27:25.000000 anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64850 2023-11-15 22:27:25.000000 anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2023-11-15 22:27:25.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2023-11-15 22:27:25.000000 anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-11-15 22:29:57.000000 anonymized_testing_data/invalid_data/mult_series_uid/
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2023-11-15 22:29:57.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64880 2023-11-15 22:29:57.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-12-06 18:46:11.000000 anonymized_testing_data/contrast_data/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-12-06 18:55:40.000000 anonymized_testing_data/contrast_data/with_contrast/
--rw-r--r--   0 cavriley (2446225) users      (100)   437476 2023-12-07 19:34:24.000000 anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2023-12-06 18:56:57.000000 anonymized_testing_data/contrast_data/without_contrast/
--rw-r--r--   0 cavriley (2446225) users      (100)   132600 2023-12-07 19:34:39.000000 anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149132 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149148 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149134 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149134 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111492 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234544 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234538 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    10135 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/flair.xml
+-rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234548 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234540 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   234538 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832602 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653406 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653406 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653404 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653398 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653398 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653404 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)    66394 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66382 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66384 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218166 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111704 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111694 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111694 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111696 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111700 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166946 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166948 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166956 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166952 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111492 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314416 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   149114 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149110 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149110 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149114 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)    66392 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66388 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)    66396 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66394 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    66382 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/
+-rw-r--r--   0 cavriley (2446225) users      (100)    13532 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/no_valid_fields.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/
+-rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64842 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64850 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/
+-rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832220 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm
+-rw-r--r--   0 cavriley (2446225) users      (100)   832220 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/all_fields_data/
+-rw-r--r--   0 cavriley (2446225) users      (100)    64900 2024-03-28 15:09:01.000000 anonymized_testing_data/all_fields_data/all_fields_file.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/with_contrast/
+-rw-r--r--   0 cavriley (2446225) users      (100)   437476 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm
+drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/without_contrast/
+-rw-r--r--   0 cavriley (2446225) users      (100)   132600 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm
```

### Comparing `dcm_classifier-0.6.0rc9/tests/testing_data/mock_data.txt` & `dcm_classifier-0.7.0rc1/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/tests/unit_testing/test_namic_dicom_typing.py` & `dcm_classifier-0.7.0rc1/tests/unit_testing/test_utility_functions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import numpy as np
 import pydicom
 import pytest
 from dcm_classifier.example_image_processing import slugify, rglob_for_singular_result
+from dcm_classifier.image_type_inference import *
+from dcm_classifier.study_processing import ProcessOneDicomStudyToVolumesMappingBase
 from dcm_classifier.utility_functions import (
     vprint,
     get_diffusion_gradient_direction,
     convert_array_to_min_max,
     sanitize_dicom_dataset,
     itk_read_from_dicomfn_list,
     is_integer,
+    ensure_magnitude_of_1,
+    convert_array_to_index_value,
+    get_coded_dictionary_elements,
 )
 from dcm_classifier.dicom_config import required_DICOM_fields, optional_DICOM_fields
 from pathlib import Path
 
 relative_testing_data_path: Path = Path(__file__).parent.parent / "testing_data"
 current_file_path: Path = Path(__file__).parent
 inference_model_path = list(
@@ -137,15 +143,15 @@
         vol.append(file)
 
     with pytest.raises(AssertionError) as ex:
         itk_read_from_dicomfn_list(vol)
     assert "Too many series in DICOMs in:" in str(ex.value)
 
 
-def test_ADC_in_image_type_field():
+def test_diff_grad_dir():
     assert dicom_file_dir.exists()
     file = list(dicom_file_dir.rglob("*.dcm"))[0]
     ds = pydicom.dcmread(file, stop_before_pixels=True)
 
     assert get_diffusion_gradient_direction(ds) is None
 
 
@@ -196,14 +202,87 @@
 
     f = pydicom.dcmread(vol[0])
     ds_dict = sanitize_dicom_dataset(f, required_DICOM_fields, optional_DICOM_fields)[0]
 
     assert ds_dict["PixelBandwidth"] == "INVALID_VALUE"
 
 
+def test_invalid_fields():
+    file_dir = dicom_file_dir.parent
+
+    assert file_dir.exists()
+    vol = list()
+    for file in file_dir.iterdir():
+        if "no_valid" in file.stem:
+            vol.append(file)
+
+    f = pydicom.dcmread(vol[0])
+    ds_dict = sanitize_dicom_dataset(f, required_DICOM_fields, optional_DICOM_fields)[0]
+
+    # Convert all values to strings
+    ds_dict = {str(field): str(value) for field, value in ds_dict.items()}
+
+    all_fields = required_DICOM_fields + optional_DICOM_fields
+    all_fields = [
+        field
+        for field in all_fields
+        if field
+        not in [
+            "Diffusionb-value",
+            "Diffusionb-valueMax",
+            "StudyInstanceUID",
+            "SeriesInstanceUID",
+            "FileName",
+            "list_of_ordered_volume_files",
+        ]
+    ]
+
+    # assert the fields that are in the dataset are set to one of these invalid values
+    invalid_fields = ["INVALID_VALUE", "-12345", "Unknown", "-12345.0", "None", ""]
+    for field in all_fields:
+        print(field, ds_dict[field])
+        if "unknown" in ds_dict[field].lower():
+            assert True
+        else:
+            assert ds_dict[field] in invalid_fields
+
+
+def test_run_inference_validate_features(get_data_dir):
+    dwi_directory = get_data_dir.parent / "anonymized_dwi_series"
+    assert dwi_directory.exists()
+
+    # run study on anonymized data
+    inferer = ImageTypeClassifierBase(
+        classification_model_filename=inference_model_path
+    )
+    study = ProcessOneDicomStudyToVolumesMappingBase(
+        study_directory=dwi_directory, inferer=inferer
+    )
+
+    # remove the fields that are validated in the inference
+
+    for series_num, series in study.series_dictionary.items():
+        for vol in series.get_volume_list():
+            del vol.__getattribute__("volume_info_dict")["ImageType"]
+            del vol.__getattribute__("volume_info_dict")["SeriesNumber"]
+            del vol.__getattribute__("volume_info_dict")["EchoTime"]
+            del vol.__getattribute__("volume_info_dict")["PixelBandwidth"]
+
+    study.run_inference()
+
+    for series_num, series in study.series_dictionary.items():
+        # print(
+        #     ImageTypeClassifierBase.infer_modality(
+        #         series.get_volume_list()[0].get_volume_dictionary()
+        #     )
+        # )
+        for vol in series.get_volume_list():
+            assert vol.get_volume_modality() == "INVALID"
+
+
 # def test_invalid_fields():
 #     assert dicom_file_dir.exists()
 #     vol = list()
 #     for file in dicom_file_dir.iterdir():
 #         if "invalid" in file.stem:
 #             vol.append(file)
 #
@@ -223,11 +302,59 @@
 #     # Tests dicom file with an empty pixel bandwidth field
 #     f = pydicom.dcmread(vol[2])
 #     with pytest.raises(TypeError) as ex:
 #         ds_dict = sanitize_dicom_dataset(f, required_DICOM_fields, optional_DICOM_fields)[0]
 #     assert "not 'NoneType'" in str(ex.value)
 
 
+def test_unit_vector():
+    vec: np.ndarray = np.array([1 / np.sqrt(3), 1 / np.sqrt(3), 1 / np.sqrt(3)])
+
+    assert ensure_magnitude_of_1(vec) is True
+
+    vec = np.array([1, 1, 1])
+    assert ensure_magnitude_of_1(vec) is False
+
+
+def test_get_gradient_direction(get_data_dir):
+    # testing no gradient, not dwi series
+    no_grad_dir = get_data_dir / "1" / "DICOM"
+    no_grad = list(no_grad_dir.rglob("*.dcm"))[0]
+    ds = pydicom.dcmread(no_grad)
+    assert get_diffusion_gradient_direction(ds) is None
+
+    # testing gradient direction
+    grad_dir = get_data_dir.parent / "anonymized_dwi_series" / "DICOM"
+    grad = list(grad_dir.rglob("*.dcm"))[0]
+    ds_w_grad = pydicom.dcmread(grad)
+
+    # ensure each element in the diffusion gradient direction is equal to the value in the DICOM header
+    for elem in zip(
+        get_diffusion_gradient_direction(ds_w_grad), ds_w_grad[(0x0019, 0x100E)].value
+    ):
+        assert elem[0] == elem[1]
+
+
 def test_is_integer():
     assert is_integer("1") is True
     assert is_integer("test") is False
     assert is_integer("1.0") is False
+
+
+def test_conv_arr_to_index_val():
+    arr = "yes//this//is//a//test"
+    with pytest.raises(ValueError) as ex:
+        convert_array_to_index_value("test", arr)
+    assert "could not convert string to float" in str(ex.value)
+
+
+def test_get_invalid_coded_dictionary():
+    test_dict = {"example_value": "INVALID_VALUE"}
+
+    assert get_coded_dictionary_elements(test_dict) == {}
+
+
+def test_get_EADC_image_type():
+    test_dict = {"ImageType": ["ORIGINAL", "PRIMARY", "EADC", "NONE"]}
+
+    assert get_coded_dictionary_elements(test_dict)["ImageType_EADC"] == 1
+
```

### Comparing `dcm_classifier-0.6.0rc9/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.7.0rc1/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/.gitignore` & `dcm_classifier-0.7.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/LICENSE` & `dcm_classifier-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/README.md` & `dcm_classifier-0.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.6.0rc9/pyproject.toml` & `dcm_classifier-0.7.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.6.0.rc9'
+version = '0.7.0.rc1'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.2"
```

### Comparing `dcm_classifier-0.6.0rc9/PKG-INFO` & `dcm_classifier-0.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.6.0rc9
+Version: 0.7.0rc1
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Introduction
 
 In this work, we developed a robust, easily extensible classification framework that extracts key features from well-characterized DICOM header fields for identifying image modality and acquisition plane. Our tool is crucial for eliminating error-prone human interaction and allowing automatization, increasing imaging applications' reliability and efficiency. We used Random Forrest and Decision Tree algorithms to determine the image modality and orientation. We trained on header meta-data of over 49000 scan volumes from multiple studies and achieved over 99% prediction accuracy on image modality and acquisition plane classification.
 
 This project was supported by several funding sources including:
```

