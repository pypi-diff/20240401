# Comparing `tmp/mbari_pbp-0.3.0b8.tar.gz` & `tmp/mbari_pbp-0.3.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbari_pbp-0.3.0b8.tar", max compression
+gzip compressed data, was "mbari_pbp-0.3.0b9.tar", max compression
```

## Comparing `mbari_pbp-0.3.0b8.tar` & `mbari_pbp-0.3.0b9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2323 2024-03-29 17:12:25.782657 mbari_pbp-0.3.0b8/README.md
--rw-r--r--   0        0        0      713 2024-03-20 17:08:11.145164 mbari_pbp-0.3.0b8/pbp/__init__.py
--rw-r--r--   0        0        0    18725 2024-03-19 19:18:59.482843 mbari_pbp-0.3.0b8/pbp/file_helper.py
--rw-r--r--   0        0        0        0 2024-03-19 19:18:59.483832 mbari_pbp-0.3.0b8/pbp/json_generator/__init__.py
--rw-r--r--   0        0        0    11008 2024-03-19 20:03:51.005509 mbari_pbp-0.3.0b8/pbp/json_generator/corrector.py
--rw-r--r--   0        0        0     1912 2024-03-19 19:18:59.485225 mbari_pbp-0.3.0b8/pbp/json_generator/gen_abstract.py
--rw-r--r--   0        0        0     9130 2024-03-19 20:03:51.024088 mbari_pbp-0.3.0b8/pbp/json_generator/gen_iclisten.py
--rw-r--r--   0        0        0     7913 2024-03-29 21:56:57.723311 mbari_pbp-0.3.0b8/pbp/json_generator/gen_nrs.py
--rw-r--r--   0        0        0     8266 2024-03-19 20:03:51.019869 mbari_pbp-0.3.0b8/pbp/json_generator/gen_soundtrap.py
--rwxr-xr-x   0        0        0    10079 2024-03-19 19:18:59.486728 mbari_pbp-0.3.0b8/pbp/json_generator/metadata_extractor.py
--rw-r--r--   0        0        0      317 2024-03-19 19:18:59.486940 mbari_pbp-0.3.0b8/pbp/json_generator/utils.py
--rw-r--r--   0        0        0     4285 2024-03-19 19:18:59.487207 mbari_pbp-0.3.0b8/pbp/json_support.py
--rw-r--r--   0        0        0     2603 2024-03-19 19:18:59.487417 mbari_pbp-0.3.0b8/pbp/logging_helper.py
--rw-r--r--   0        0        0     2550 2024-03-19 21:40:24.439066 mbari_pbp-0.3.0b8/pbp/main.py
--rw-r--r--   0        0        0     4746 2024-03-19 21:40:24.442493 mbari_pbp-0.3.0b8/pbp/main_args.py
--rw-r--r--   0        0        0     7041 2024-03-19 19:18:59.488974 mbari_pbp-0.3.0b8/pbp/main_cloud.py
--rw-r--r--   0        0        0     2376 2024-03-19 19:18:59.489349 mbari_pbp-0.3.0b8/pbp/main_json_generator.py
--rw-r--r--   0        0        0     2430 2024-03-28 22:52:21.345070 mbari_pbp-0.3.0b8/pbp/main_json_generator_args.py
--rw-r--r--   0        0        0     2563 2024-03-19 19:18:59.489979 mbari_pbp-0.3.0b8/pbp/metadata.py
--rw-r--r--   0        0        0     2075 2024-03-19 19:18:59.490207 mbari_pbp-0.3.0b8/pbp/misc_helper.py
--rw-r--r--   0        0        0     2823 2024-03-19 20:11:16.990989 mbari_pbp-0.3.0b8/pbp/plot.py
--rw-r--r--   0        0        0      296 2024-03-19 19:18:59.490840 mbari_pbp-0.3.0b8/pbp/plot_const.py
--rw-r--r--   0        0        0     5047 2024-03-19 19:18:59.491113 mbari_pbp-0.3.0b8/pbp/plotting.py
--rw-r--r--   0        0        0    12492 2024-03-20 17:07:17.364246 mbari_pbp-0.3.0b8/pbp/process_helper.py
--rw-r--r--   0        0        0    10014 2024-03-19 19:18:59.491862 mbari_pbp-0.3.0b8/pbp/pypam_support.py
--rw-r--r--   0        0        0     1470 2024-03-29 21:56:57.728260 mbari_pbp-0.3.0b8/pyproject.toml
--rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 mbari_pbp-0.3.0b8/PKG-INFO
+-rw-r--r--   0        0        0     2700 2024-04-01 18:07:40.327845 mbari_pbp-0.3.0b9/README.md
+-rw-r--r--   0        0        0      713 2024-03-20 17:08:11.145164 mbari_pbp-0.3.0b9/pbp/__init__.py
+-rw-r--r--   0        0        0    18725 2024-03-19 19:18:59.482843 mbari_pbp-0.3.0b9/pbp/file_helper.py
+-rw-r--r--   0        0        0        0 2024-03-19 19:18:59.483832 mbari_pbp-0.3.0b9/pbp/json_generator/__init__.py
+-rw-r--r--   0        0        0    11008 2024-03-19 20:03:51.005509 mbari_pbp-0.3.0b9/pbp/json_generator/corrector.py
+-rw-r--r--   0        0        0     1941 2024-04-01 17:58:44.149037 mbari_pbp-0.3.0b9/pbp/json_generator/gen_abstract.py
+-rw-r--r--   0        0        0     9159 2024-04-01 17:58:44.160810 mbari_pbp-0.3.0b9/pbp/json_generator/gen_iclisten.py
+-rw-r--r--   0        0        0     7858 2024-04-01 18:40:28.347261 mbari_pbp-0.3.0b9/pbp/json_generator/gen_nrs.py
+-rw-r--r--   0        0        0     8294 2024-04-01 17:58:44.155920 mbari_pbp-0.3.0b9/pbp/json_generator/gen_soundtrap.py
+-rwxr-xr-x   0        0        0    10079 2024-03-19 19:18:59.486728 mbari_pbp-0.3.0b9/pbp/json_generator/metadata_extractor.py
+-rw-r--r--   0        0        0      347 2024-04-01 17:55:57.413221 mbari_pbp-0.3.0b9/pbp/json_generator/utils.py
+-rw-r--r--   0        0        0     4285 2024-03-19 19:18:59.487207 mbari_pbp-0.3.0b9/pbp/json_support.py
+-rw-r--r--   0        0        0     2603 2024-03-19 19:18:59.487417 mbari_pbp-0.3.0b9/pbp/logging_helper.py
+-rw-r--r--   0        0        0     2550 2024-03-19 21:40:24.439066 mbari_pbp-0.3.0b9/pbp/main.py
+-rw-r--r--   0        0        0     4746 2024-03-19 21:40:24.442493 mbari_pbp-0.3.0b9/pbp/main_args.py
+-rw-r--r--   0        0        0     7041 2024-03-19 19:18:59.488974 mbari_pbp-0.3.0b9/pbp/main_cloud.py
+-rw-r--r--   0        0        0     2376 2024-03-19 19:18:59.489349 mbari_pbp-0.3.0b9/pbp/main_json_generator.py
+-rw-r--r--   0        0        0     2430 2024-03-28 22:52:21.345070 mbari_pbp-0.3.0b9/pbp/main_json_generator_args.py
+-rw-r--r--   0        0        0     2563 2024-03-19 19:18:59.489979 mbari_pbp-0.3.0b9/pbp/metadata.py
+-rw-r--r--   0        0        0     2075 2024-03-19 19:18:59.490207 mbari_pbp-0.3.0b9/pbp/misc_helper.py
+-rw-r--r--   0        0        0     2823 2024-03-19 20:11:16.990989 mbari_pbp-0.3.0b9/pbp/plot.py
+-rw-r--r--   0        0        0      296 2024-03-19 19:18:59.490840 mbari_pbp-0.3.0b9/pbp/plot_const.py
+-rw-r--r--   0        0        0     5047 2024-03-19 19:18:59.491113 mbari_pbp-0.3.0b9/pbp/plotting.py
+-rw-r--r--   0        0        0    12492 2024-03-20 17:07:17.364246 mbari_pbp-0.3.0b9/pbp/process_helper.py
+-rw-r--r--   0        0        0    10014 2024-03-19 19:18:59.491862 mbari_pbp-0.3.0b9/pbp/pypam_support.py
+-rw-r--r--   0        0        0     1570 2024-04-01 18:39:31.357159 mbari_pbp-0.3.0b9/pyproject.toml
+-rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 mbari_pbp-0.3.0b9/PKG-INFO
```

### Comparing `mbari_pbp-0.3.0b8/pbp/__init__.py` & `mbari_pbp-0.3.0b9/pbp/__init__.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/file_helper.py` & `mbari_pbp-0.3.0b9/pbp/file_helper.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/json_generator/corrector.py` & `mbari_pbp-0.3.0b9/pbp/json_generator/corrector.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/json_generator/gen_abstract.py` & `mbari_pbp-0.3.0b9/pbp/json_generator/gen_abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # pypam-based-processing
 # Filename: metadata/generator/gen_abstract.py
 # Description:  Abstract class that captures sound wav metadata
 from datetime import datetime
+from typing import List
+
 import pandas as pd
 from pbp.logging_helper import PbpLogger
 
 
 class MetadataGeneratorAbstract(object):
     def __init__(
         self,
         logger: PbpLogger,
         audio_loc: str,
         json_base_dir: str,
-        prefix: [str],
+        prefix: List[str],
         start: datetime,
         end: datetime,
         seconds_per_file: float = 0.0,
         **kwargs,
     ):
         """
         Abstract class for capturing sound wav metadata
```

### Comparing `mbari_pbp-0.3.0b8/pbp/json_generator/gen_iclisten.py` & `mbari_pbp-0.3.0b9/pbp/json_generator/gen_iclisten.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pypam-based-processing, Apache License 2.0
 # Filename: metadata/generator/gen_iclisten.py
 # Description:  Captures ICListen wav metadata in a pandas dataframe from either a local directory or S3 bucket.
 
 import re
 from datetime import timedelta
 from datetime import datetime
+from typing import List
+
 import boto3
 
 import pandas as pd
 from pathlib import Path
 from progressbar import progressbar
 import pbp.json_generator.utils as utils
 from pbp.json_generator.corrector import MetadataCorrector
@@ -23,15 +25,15 @@
     def __init__(
         self,
         pbp_logger: PbpLogger,
         uri: str,
         json_base_dir: str,
         start: datetime,
         end: datetime,
-        prefix: [str],
+        prefix: List[str],
         seconds_per_file: float = 300.0,
     ):
         """
         Captures ICListen wav metadata in a pandas dataframe from either a local directory or S3 bucket.
         :param pbp_logger:
             The logger
         :param uri:
```

### Comparing `mbari_pbp-0.3.0b8/pbp/json_generator/gen_nrs.py` & `mbari_pbp-0.3.0b9/pbp/json_generator/gen_nrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pypam-based-processing, Apache License 2.0
 # Filename: metadata/generator/gen_nrs.py
 # Description:  Captures NRS flac metadata in a pandas dataframe from either a local directory or gs bucket.
 
 import re
 from datetime import timedelta, datetime
 import time
+from typing import List
+
 from google.cloud import storage
 
 import pandas as pd
 from pathlib import Path
 from progressbar import progressbar
 from pbp.json_generator.corrector import MetadataCorrector
 from pbp.json_generator.metadata_extractor import FlacFile
@@ -21,15 +23,15 @@
     def __init__(
         self,
         pbp_logger: PbpLogger,
         uri: str,
         json_base_dir: str,
         start: datetime,
         end: datetime,
-        prefix: [str],
+        prefix: List[str],
         seconds_per_file: float = 14400.0,
     ):
         """
         Captures NRS audio metadata in a pandas dataframe from either a local directory or GS bucket.
         :param pbp_logger:
             The logger
         :param uri:
@@ -101,19 +103,15 @@
             f"Searching in {self.audio_loc}/ for files that match the search pattern {self.prefix}* ..."
         )
 
         # set the window to 1 flac file to account for any missing data
         minutes_window = int(self.seconds_per_file / 60)
 
         # set the start and end dates to 1 hour before and after the start and end dates
-        start_dt = (
-            self.start
-            - timedelta(minutes=minutes_window)
-            - timedelta(minutes=minutes_window)
-        )
+        start_dt = self.start - timedelta(minutes=minutes_window)
         end_dt = self.end + timedelta(days=1)
 
         if scheme == "file" or scheme == "":
             flac_path = Path(f"/{bucket}/{prefix}")
             for filename in progressbar(
                 sorted(flac_path.rglob("*.flac")), prefix="Searching : "
             ):
```

### Comparing `mbari_pbp-0.3.0b8/pbp/json_generator/gen_soundtrap.py` & `mbari_pbp-0.3.0b9/pbp/json_generator/gen_soundtrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pypam-based-processing
 # Filename: json_generator/gen_soundtrap.py
 # Description:  Captures SoundTrap metadata either from a local directory of S3 bucket
 import logging
+from typing import List
 
 import boto3
 import datetime
 import pandas as pd
 import re
 import pytz
 
@@ -30,15 +31,15 @@
     end = datetime.datetime.now(pytz.utc)
 
     def __init__(
         self,
         pbp_logger: PbpLogger,
         uri: str,
         json_base_dir: str,
-        prefix: [str],
+        prefix: List[str],
         start: datetime,
         end: datetime,
     ):
         """
         :param pbp_logger:
             The logger
         :param uri:
```

### Comparing `mbari_pbp-0.3.0b8/pbp/json_generator/metadata_extractor.py` & `mbari_pbp-0.3.0b9/pbp/json_generator/metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/json_support.py` & `mbari_pbp-0.3.0b9/pbp/json_support.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/logging_helper.py` & `mbari_pbp-0.3.0b9/pbp/logging_helper.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/main.py` & `mbari_pbp-0.3.0b9/pbp/main.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/main_args.py` & `mbari_pbp-0.3.0b9/pbp/main_args.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/main_cloud.py` & `mbari_pbp-0.3.0b9/pbp/main_cloud.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/main_json_generator.py` & `mbari_pbp-0.3.0b9/pbp/main_json_generator.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/main_json_generator_args.py` & `mbari_pbp-0.3.0b9/pbp/main_json_generator_args.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/metadata.py` & `mbari_pbp-0.3.0b9/pbp/metadata.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/misc_helper.py` & `mbari_pbp-0.3.0b9/pbp/misc_helper.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/plot.py` & `mbari_pbp-0.3.0b9/pbp/plot.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/plotting.py` & `mbari_pbp-0.3.0b9/pbp/plotting.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/process_helper.py` & `mbari_pbp-0.3.0b9/pbp/process_helper.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pbp/pypam_support.py` & `mbari_pbp-0.3.0b9/pbp/pypam_support.py`

 * *Files identical despite different names*

### Comparing `mbari_pbp-0.3.0b8/pyproject.toml` & `mbari_pbp-0.3.0b9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mbari-pbp"
-version = "0.3.0b8"
+version = "0.3.0b9"
 # for now, pbp version "aligned" (not necessarily exactly) with that of lifewatch-pypam.
 description = "PyPAM based Processing"
 authors = [
     "Carlos Rueda <carueda@mbari.org>",
     "Danelle Cline <dcline@mbari.org>",
 ]
 license = "MIT"
@@ -48,16 +48,18 @@
 
 [tool.mypy]
 show_error_codes = true
 ignore_missing_imports = true
 exclude = [
     'examples/',
     'pbp/plotting\.py',
-    'pbp/json_generator/',
-    'tests/test_json_generator.py',
+    'pbp/json_generator/metadata.*\.py',
+    'pbp/json_generator/corrector\.py',
+    'pbp/json_generator/gen_soundtrap\.py',
+    'pbp/json_generator/gen_nrs\.py',
 ]
 
 [tool.ruff]
 line-length = 90
 exclude = [
   "virtenv/**"
 ]
```

### Comparing `mbari_pbp-0.3.0b8/PKG-INFO` & `mbari_pbp-0.3.0b9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbari-pbp
-Version: 0.3.0b8
+Version: 0.3.0b9
 Summary: PyPAM based Processing
 Home-page: https://github.com/mbari-org/pbp
 License: MIT
 Author: Carlos Rueda
 Author-email: carueda@mbari.org
 Requires-Python: >=3.9,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
@@ -31,50 +31,59 @@
 
 The [`mbari-pbp`](https://pypi.org/project/mbari-pbp/) package allows to
 process ocean audio data archives to daily analysis products of hybrid millidecade spectra using
 [PyPAM](https://github.com/lifewatch/pypam/).
 
 **Status**: Functional version, including support for cloud based processing.
 
-- [x] JSON generation of timekeeping
-- [x] Timekeeping based on given JSON indicating start and duration of every available (recognized) sound file
+- [x] JSON generation of timekeeping with indication of start and duration of recognized sound files
 - [x] Audio file processing
     - [x] Frequency and psd array output
     - [x] Concatenation of processed 1-minute segments for daily product
-    - [x] Calibration with given sensitivity file (NetCDF)
-    - [x] Calibration with given flat sensitivity value
+    - [x] Calibration with given sensitivity file (NetCDF), or flat sensitivity value
 - [x] Data products
     - [x] NetCDF with metadata
     - [x] Summary plot
 - [x] Cloud processing
-    - [x] Inputs can be downloaded from S3
-    - [x] Outputs can be uploaded to S3
+    - [x] Inputs can be downloaded from and uploaded to S3
     - [x] Inputs can be downloaded from public GCS bucket
     - [ ] Outputs can be uploaded to GCS
 
 TODO more details
 
-## Setup
+## Installation
 
-### Install PBP
+The only requirement is Python 3.9, 3.10, or 3.11 on your environment.[^1]
+You can run `python3 --version` to check the version of Python installed.
 
-    pip install mbari-pbp
+[^1]: As currently [required by PyPAM](https://github.com/lifewatch/pypam/blob/29e82f0c5c6ce43b457d76963cb9d82392740654/pyproject.toml#L16).
 
-### Programs
+As a general practice, it is recommended to use a virtual environment for the installation.
+```shell
+python3.9 -m venv virtenv
+source virtenv/bin/activate
+```
+
+Install the package:
+```shell
+pip install mbari-pbp
+```
+
+## Programs
 
 The package includes the following CLI programs:
 
 | Program | Description                                    |
 | ------- |------------------------------------------------|
 | [`pbp-json-gen`](pbp-json-gen/) | Generate JSON files with audio metadata.       |
 | [`pbp`](pbp/) | Main HMB generation program.                   |
 | [`pbp-cloud`](pbp-cloud/) | Program for cloud based processing.            |
 | [`pbp-plot`](pbp-plot/) | Utility program to plot resulting HMB product. |
 
-## Refs
+## References
 
 - PyPAM - Python tool for Passive Acoustic Monitoring –
   <https://doi.org/10.5281/zenodo.6044593>
 - Computation of single-sided mean-square sound pressure spectral density with 1 Hz resolution follows
   ISO 18405 3.1.3.13 (International Standard ISO 18405:2017(E), Underwater Acoustics – Terminology. Geneva: ISO)
   – https://www.iso.org/standard/62406.html
 - Hybrid millidecade spectra: A practical format for exchange of long-term ambient sound data –
```

