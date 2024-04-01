# Comparing `tmp/smaht_submitr-0.7.0.1b7.tar.gz` & `tmp/smaht_submitr-0.7.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b7.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.1b9.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b7.tar` & `smaht_submitr-0.7.0.1b9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1098 2024-03-20 18:06:20.206426 smaht_submitr-0.7.0.1b7/LICENSE.txt
--rw-r--r--   0        0        0     2772 2024-03-20 18:06:20.206426 smaht_submitr-0.7.0.1b7/README.rst
--rw-r--r--   0        0        0     3447 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/base.py
--rw-r--r--   0        0        0      294 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/output.py
--rw-r--r--   0        0        0        0 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     3677 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     4610 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1775 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5252 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    16175 2024-03-20 18:06:20.242426 smaht_submitr-0.7.0.1b7/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    26913 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   133280 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11277 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   156743 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6796 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0     6727 2024-03-20 18:06:20.246426 smaht_submitr-0.7.0.1b7/submitr/utils.py
--rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b7/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-03-20 18:15:36.180092 smaht_submitr-0.7.0.1b9/LICENSE.txt
+-rw-r--r--   0        0        0     2601 2024-03-20 18:15:36.180092 smaht_submitr-0.7.0.1b9/README.rst
+-rw-r--r--   0        0        0     3447 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/output.py
+-rw-r--r--   0        0        0        0 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     3677 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     4610 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1775 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5252 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    16175 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    26913 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   133280 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11277 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-03-20 18:15:36.220093 smaht_submitr-0.7.0.1b9/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   156743 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6796 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0     6727 2024-03-20 18:15:36.224094 smaht_submitr-0.7.0.1b9/submitr/utils.py
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b9/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b7/LICENSE.txt` & `smaht_submitr-0.7.0.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/README.rst` & `smaht_submitr-0.7.0.1b9/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 .. image:: https://staging.smaht.org/static/img/docs/submitr_logo.png
     :target: https://pypi.org/project/smaht-submitr/
     :alt: SMaHT remote Metadata Submission Tool: submitr
     :align: left
 
+
 |
 
+
 ------------
 
 ==============
 smaht-submitr
 ==============
 
 
@@ -20,25 +22,26 @@
    :target: https://github.com/smaht-dac/submitr/actions
    :alt: Build Status
 
 .. image:: https://coveralls.io/repos/github/smaht-dac/submitr/badge.svg
     :target: https://coveralls.io/github/smaht-dac/submitr
     :alt: Coverage Percentage
 
-.. image:: https://readthedocs.org/projects/submitr/badge/?version=latest
-   :target: https://submitr.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/submitr/badge/?version=draft
+   :target: https://submitr.readthedocs.io/en/draft/?badge=draft
    :alt: Documentation Status
 
 
 Description
 ===========
 
 This is a tool for uploading certain kinds of files to SMaHT.
 The "R" is for Remote file submission. You can think of this tool as putting the "R" in "SMaHT". :)
-Please see our detailed documentation here: https://submitr.readthedocs.io/en/draft/
+
+Please see our detailed documentation here: `SMaHT Submitr <https://submitr.readthedocs.io/en/draft/>`_
 
 
 Background
 ==========
 
 This tool was forked from SubmitCGAP and will probably remain compatible, but by forking it, the original repository will remain stable and this new repository can experiment safely.
 
@@ -46,38 +49,21 @@
 
 
 Installation
 ============
 
 Installing this system involves these steps:
 
-1. Create, install, and activate a virtual environment.
-2. *Only if you are a developer*, install poetry and select the source repository.
-   Others will not have a source repository to select,
-   so should skip this step.
-3. If you are an end user, do "``pip install smaht-submitr``".
-   Otherwise, do "``make build``".
-4. Set up a ``~/.smaht-keys.json`` credentials file.
-
-See detailed information about these installation steps at
-`Installing submitr <https://submitr.readthedocs.io/en/latest/installation.html>`_.
-
-
-
-Testing
-=======
-
-To run unit tests, do::
-
-   $ make test
+1. Install Python and optionally a virtual environment manager of your choice (e.g. ``pyenv``)..
+3. Install this package with: ``pip install smaht-submitr``
+4. Setup your SMaHT Portal credentials file: ``~/.smaht-keys.json``. See `SMaHT Submitr Credentals <https://submitr.readthedocs.io/en/draft/installation.html>`_ for more in this.
 
-Additional notes on testing these scripts for release can be found in
-`Testing submitr <TESTING.rst>`__.
+See detailed information about installation see: `Installing SMaHT Submitr <https://submitr.readthedocs.io/en/draft/installation.html>`_.
 
 
 Getting Started
 ===============
 
 Once you have finished installing this library into your virtual environment,
 you should have access to the ``submit-metadata-bundle``, ``resume-uploads``, and ``check-submissions``
 commands. For more information about how to format files for submission and how to
-use these commands, see `Getting Started <https://submitr.readthedocs.io/en/draft/usage.html>`_.
+use these commands, see `Getting Started with SMaHT Submitr <https://submitr.readthedocs.io/en/draft/usage.html>`_.
```

### Comparing `smaht_submitr-0.7.0.1b7/pyproject.toml` & `smaht_submitr-0.7.0.1b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b7"  # TODO: To become 0.8.0
+version = "0.7.0.1b9"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.1b7/submitr/base.py` & `smaht_submitr-0.7.0.1b9/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/output.py` & `smaht_submitr-0.7.0.1b9/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.1b9/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/submission.py` & `smaht_submitr-0.7.0.1b9/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.1b9/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.1b9/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/submitr/utils.py` & `smaht_submitr-0.7.0.1b9/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b7/PKG-INFO` & `smaht_submitr-0.7.0.1b9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b7
+Version: 0.7.0.1b9
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
@@ -34,16 +34,18 @@
 
 
 .. image:: https://staging.smaht.org/static/img/docs/submitr_logo.png
     :target: https://pypi.org/project/smaht-submitr/
     :alt: SMaHT remote Metadata Submission Tool: submitr
     :align: left
 
+
 |
 
+
 ------------
 
 ==============
 smaht-submitr
 ==============
 
 
@@ -54,25 +56,26 @@
    :target: https://github.com/smaht-dac/submitr/actions
    :alt: Build Status
 
 .. image:: https://coveralls.io/repos/github/smaht-dac/submitr/badge.svg
     :target: https://coveralls.io/github/smaht-dac/submitr
     :alt: Coverage Percentage
 
-.. image:: https://readthedocs.org/projects/submitr/badge/?version=latest
-   :target: https://submitr.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/submitr/badge/?version=draft
+   :target: https://submitr.readthedocs.io/en/draft/?badge=draft
    :alt: Documentation Status
 
 
 Description
 ===========
 
 This is a tool for uploading certain kinds of files to SMaHT.
 The "R" is for Remote file submission. You can think of this tool as putting the "R" in "SMaHT". :)
-Please see our detailed documentation here: https://submitr.readthedocs.io/en/draft/
+
+Please see our detailed documentation here: `SMaHT Submitr <https://submitr.readthedocs.io/en/draft/>`_
 
 
 Background
 ==========
 
 This tool was forked from SubmitCGAP and will probably remain compatible, but by forking it, the original repository will remain stable and this new repository can experiment safely.
 
@@ -80,39 +83,22 @@
 
 
 Installation
 ============
 
 Installing this system involves these steps:
 
-1. Create, install, and activate a virtual environment.
-2. *Only if you are a developer*, install poetry and select the source repository.
-   Others will not have a source repository to select,
-   so should skip this step.
-3. If you are an end user, do "``pip install smaht-submitr``".
-   Otherwise, do "``make build``".
-4. Set up a ``~/.smaht-keys.json`` credentials file.
-
-See detailed information about these installation steps at
-`Installing submitr <https://submitr.readthedocs.io/en/latest/installation.html>`_.
-
-
-
-Testing
-=======
-
-To run unit tests, do::
-
-   $ make test
+1. Install Python and optionally a virtual environment manager of your choice (e.g. ``pyenv``)..
+3. Install this package with: ``pip install smaht-submitr``
+4. Setup your SMaHT Portal credentials file: ``~/.smaht-keys.json``. See `SMaHT Submitr Credentals <https://submitr.readthedocs.io/en/draft/installation.html>`_ for more in this.
 
-Additional notes on testing these scripts for release can be found in
-`Testing submitr <TESTING.rst>`__.
+See detailed information about installation see: `Installing SMaHT Submitr <https://submitr.readthedocs.io/en/draft/installation.html>`_.
 
 
 Getting Started
 ===============
 
 Once you have finished installing this library into your virtual environment,
 you should have access to the ``submit-metadata-bundle``, ``resume-uploads``, and ``check-submissions``
 commands. For more information about how to format files for submission and how to
-use these commands, see `Getting Started <https://submitr.readthedocs.io/en/draft/usage.html>`_.
+use these commands, see `Getting Started with SMaHT Submitr <https://submitr.readthedocs.io/en/draft/usage.html>`_.
```

