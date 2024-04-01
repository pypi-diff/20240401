# Comparing `tmp/nbiatoolkit-1.0.1.tar.gz` & `tmp/nbiatoolkit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbiatoolkit-1.0.1.tar", max compression
+gzip compressed data, was "nbiatoolkit-1.2.0.tar", max compression
```

## Comparing `nbiatoolkit-1.0.1.tar` & `nbiatoolkit-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rwxr-xr-x   0        0        0     1072 2024-03-16 21:19:07.305244 nbiatoolkit-1.0.1/LICENSE
--rw-r--r--   0        0        0     7332 2024-03-16 21:19:07.305244 nbiatoolkit-1.0.1/README.md
--rw-r--r--   0        0        0     2191 2024-03-16 21:19:51.201396 nbiatoolkit-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      664 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/__init__.py
--rw-r--r--   0        0        0    10005 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/auth.py
--rw-r--r--   0        0        0      429 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/dicomsort/__init__.py
--rw-r--r--   0        0        0    10744 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/dicomsort/dicomsort.py
--rw-r--r--   0        0        0     2218 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/dicomsort/helper_functions.py
--rw-r--r--   0        0        0     2571 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/logger/README.md
--rw-r--r--   0        0        0       61 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/logger/__init__.py
--rw-r--r--   0        0        0     2755 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/logger/logger.py
--rw-r--r--   0        0        0    23619 2024-03-16 21:19:36.309338 nbiatoolkit-1.0.1/src/nbiatoolkit/nbia.py
--rw-r--r--   0        0        0    14798 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/nbia_cli.py
--rw-r--r--   0        0        0      463 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/utils/__init__.py
--rw-r--r--   0        0        0     1001 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/utils/conv_response_list.py
--rw-r--r--   0        0        0     1222 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/utils/md5.py
--rw-r--r--   0        0        0     1742 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/utils/nbia_endpoints.py
--rw-r--r--   0        0        0     3785 2024-03-16 21:19:07.309244 nbiatoolkit-1.0.1/src/nbiatoolkit/utils/parsers.py
--rw-r--r--   0        0        0     8122 1970-01-01 00:00:00.000000 nbiatoolkit-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2024-04-01 18:00:32.609818 nbiatoolkit-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6862 2024-04-01 18:00:32.609818 nbiatoolkit-1.2.0/README.md
+-rw-r--r--   0        0        0     2203 2024-04-01 18:00:32.613818 nbiatoolkit-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      664 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/__init__.py
+-rw-r--r--   0        0        0    10005 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/auth.py
+-rw-r--r--   0        0        0      429 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/dicomsort/__init__.py
+-rw-r--r--   0        0        0    10744 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/dicomsort/dicomsort.py
+-rw-r--r--   0        0        0     2218 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/dicomsort/helper_functions.py
+-rw-r--r--   0        0        0      500 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/dicomtags/__init__.py
+-rw-r--r--   0        0        0    10882 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/dicomtags/tags.py
+-rw-r--r--   0        0        0     2571 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/logger/README.md
+-rw-r--r--   0        0        0       61 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/logger/__init__.py
+-rw-r--r--   0        0        0     2755 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/logger/logger.py
+-rw-r--r--   0        0        0    24133 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/nbia.py
+-rw-r--r--   0        0        0    14799 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/nbia_cli.py
+-rw-r--r--   0        0        0      463 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/utils/conv_response_list.py
+-rw-r--r--   0        0        0     1222 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/utils/md5.py
+-rw-r--r--   0        0        0     1742 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/utils/nbia_endpoints.py
+-rw-r--r--   0        0        0     3785 2024-04-01 18:00:32.617818 nbiatoolkit-1.2.0/src/nbiatoolkit/utils/parsers.py
+-rw-r--r--   0        0        0     7702 1970-01-01 00:00:00.000000 nbiatoolkit-1.2.0/PKG-INFO
```

### Comparing `nbiatoolkit-1.0.1/LICENSE` & `nbiatoolkit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/README.md` & `nbiatoolkit-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/jjjermiah/nbia-toolkit)
 [![PyPI version](https://badge.fury.io/py/nbiatoolkit.svg)](https://badge.fury.io/py/nbiatoolkit)
 [![Downloads](https://static.pepy.tech/badge/nbiatoolkit)](https://pepy.tech/project/nbiatoolkit)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/nbiatoolkit.svg?label=pypi%20downloads)](https://pypi.org/project/nbiatoolkit/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jjjermiah/nbia-toolkit)
 [![Docker Pulls](https://img.shields.io/docker/pulls/jjjermiah/nbiatoolkit)](https://hub.docker.com/r/jjjermiah/nbiatoolkit)
 
-![GitHub milestone details](https://img.shields.io/github/milestones/progress-percent/jjjermiah/nbia-toolkit/1?style=flat-square&label=1.0.0%20Stable%20Release%20Milestone&link=https%3A%2F%2Fgithub.com%2Fjjjermiah%2Fnbia-toolkit%2Fmilestone%2F1)![GitHub milestone details](https://img.shields.io/github/milestones/progress/jjjermiah/nbia-toolkit/1?style=flat-square&label=%20&link=https%3A%2F%2Fgithub.com%2Fjjjermiah%2Fnbia-toolkit%2Fmilestone%2F1)
 [![GitHub issues](https://img.shields.io/github/issues/jjjermiah/nbia-toolkit)](https://github.com/jjjermiah/nbia-toolkit/issues)
 ![GitHub last commit](https://img.shields.io/github/last-commit/jjjermiah/nbia-toolkit)
 
 ## Table of Contents
+
 - [Features](#features)
 - [Installation](#installation)
 - [Python Usage](#python-usage)
 - [CLI Usage](#cli-usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [User Agreements and Disclaimers](#user-agreements-and-disclaimers)
@@ -39,15 +39,15 @@
   - Custom `OAuth2` class for **NBIA**, **TCIA**, including special handling for dedicated server for the **NLST** collection.
 
 - ***Query NBIA database*** for metadata on ***collections***, ***patients***, ***studies***, ***series***, and ***images***
 - Download images from NBIA
   - ***Validate doownloads with MD5 checksums*** for downloaded images
   - **Auto-sort** DICOM files using a user-defined pattern of DICOM tags with specialized ***DICOMSorter class***
 
-![SequenceDiagram](https://www.mermaidchart.com/raw/ce7f489f-bf58-4827-aedb-e379ed7bffd3?theme=dark&version=v0.1&format=svg)
+See [Developer Notes](devnotes/README.md) for more details on the features and the development process.
 
 ## Installation
 
 > [!WARNING]
 > `nbiatoolkit` is currently under development and is not guaranteed to be stable.
 
 It is made available via PyPI and can be installed using pip:
@@ -90,15 +90,15 @@
 
         _   ______  _______  ______            ____   _ __
        / | / / __ )/  _/   |/_  __/___  ____  / / /__(_) /_
       /  |/ / __  |/ // /| | / / / __ \/ __ \/ / //_/ / __/
      / /|  / /_/ // // ___ |/ / / /_/ / /_/ / / ,< / / /_
     /_/ |_/_____/___/_/  |_/_/  \____/\____/_/_/|_/_/\__/
 
-Version: 1.0.0
+Version: 1.0.1
 
 Available CLI tools:
 
 getCollections [-h] [-u USERNAME] [-pw PASSWORD] [-p PREFIX]
                [-o OUTPUTFILE] [--version]
 
 getBodyPartCounts [-h] [-u USERNAME] [-pw PASSWORD] [-c COLLECTION]
```

### Comparing `nbiatoolkit-1.0.1/pyproject.toml` & `nbiatoolkit-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nbiatoolkit"
-version = "1.0.1"
+version = "1.2.0"
 description = "A python package to query the National Biomedical Imaging Archive (NBIA) database."
 authors = ["Jermiah Joseph"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 dicomsort = "nbiatoolkit.nbia_cli:DICOMSorter_cli"
@@ -15,15 +15,15 @@
 getNewPatients = "nbiatoolkit.nbia_cli:getNewPatients_cli"
 getStudies = "nbiatoolkit.nbia_cli:getStudies_cli"
 getSeries = "nbiatoolkit.nbia_cli:getSeries_cli"
 getNewSeries = "nbiatoolkit.nbia_cli:getNewSeries_cli"
 
 
 [tool.poetry.dependencies]
-python = ">=3.10 || 3.12"
+python = ">=3.09 || 3.12"
 requests = "2.31.0"
 pydicom = "^2.4.0"
 tqdm = "^4.66.1"
 beautifulsoup4 = "^4.12.3"
 cryptography = "^42.0.2"
 pandas = "^2.2.0"
 pyarrow = "^15.0.0"
@@ -60,15 +60,15 @@
 patch_without_tag = true
 
 [tool.semantic_release.changelog]
 changelog_file = "docs/project_info/CHANGELOG.md"
 exclude_commit_types = ["docs", "style", "refactor", "test", "chore"]
 
 [tool.semantic_release.branches.main]
-match = "(main|master)"
+match = "(main|master|development)"
 
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = [
     "build",
     "chore",
     "ci",
```

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/__init__.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/auth.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/auth.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/dicomsort/dicomsort.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/dicomsort/dicomsort.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/dicomsort/helper_functions.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/dicomsort/helper_functions.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/logger/README.md` & `nbiatoolkit-1.2.0/src/nbiatoolkit/logger/README.md`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/logger/logger.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/logger/logger.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/nbia.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/nbia.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,32 @@
     clean_html,
     convertMillis,
     convertDateFormat,
     parse_response,
     ReturnType,
     conv_response_list,
 )
+
+from .dicomtags.tags import (
+    getReferencedSeriesUIDS,
+    extract_ROI_info,
+    getSequenceElement,
+)
+
 import pandas as pd
 import requests
 from requests.exceptions import JSONDecodeError as JSONDecodeError
 from typing import Union, Optional, Any, Dict, List
 import io
 import zipfile
 
 from datetime import datetime
 
 # set __version__ variable
-__version__ = "1.0.1"
+__version__ = "1.2.0"
 
 
 def downloadSingleSeries(
     SeriesInstanceUID: str,
     downloadDir: str,
     filePattern: str,
     overwrite: bool,
@@ -142,19 +149,14 @@
             else logger
         )
 
         # Setup OAuth2 client
         self._log.debug("Setting up OAuth2 client... with username %s", username)
         self._oauth2_client = OAuth2(username=username, password=password)
 
-        self._api_headers: dict[str, str] = {
-            "Authorization": f"Bearer {self._oauth2_client.access_token}",
-            "Content-Type": "application/json",
-        }
-
         self._base_url: NBIA_BASE_URLS = NBIA_BASE_URLS.NBIA
         self._return_type: ReturnType = (
             return_type
             if isinstance(return_type, ReturnType)
             else ReturnType(return_type)
         )
 
@@ -166,15 +168,21 @@
 
     @property
     def OAuth_client(self) -> OAuth2:
         return self._oauth2_client
 
     @property
     def headers(self):
-        return self._api_headers
+
+        API_HEADERS: dict[str, str] = {
+            "Authorization": f"Bearer {self.OAuth_client.access_token}",
+            "Content-Type": "application/json",
+        }
+
+        return API_HEADERS
 
     # create a setter for the base_url in case user want to use NLST
     @property
     def base_url(self) -> NBIA_BASE_URLS:
         return self._base_url
 
     @base_url.setter
@@ -610,14 +618,29 @@
         PARAMS = self.parsePARAMS({"SeriesUID": SeriesInstanceUID})
 
         response: List[dict[Any, Any]]
         response = self.query_api(endpoint=NBIA_ENDPOINTS.GET_DICOM_TAGS, params=PARAMS)
 
         return conv_response_list(response, returnType)
 
+    def getRefSeriesUIDs(
+        self,
+        SeriesInstanceUID: str,
+    ) -> List[str]:
+
+        tags_df = self.getDICOMTags(
+            SeriesInstanceUID=SeriesInstanceUID,
+            return_type=ReturnType.DATAFRAME,
+        )
+
+        if type(tags_df) != pd.DataFrame:
+            raise ValueError("DICOM Tags not df or not found in the response.")
+
+        return getReferencedSeriesUIDS(series_tags_df=tags_df)
+
     def downloadSeries(
         self,
         SeriesInstanceUID: Union[str, list],
         downloadDir: str = "./NBIA-Download",
         filePattern: str = "%PatientName/%Modality-%SeriesNumber-%SeriesInstanceUID/%InstanceNumber.dcm",
         overwrite: bool = False,
         nParallel: int = 1,
@@ -635,15 +658,15 @@
             result = pool.apply_async(
                 func=downloadSingleSeries,
                 args=(
                     series,
                     downloadDir,
                     filePattern,
                     overwrite,
-                    self._api_headers,
+                    self.headers,
                     self._base_url,
                     self._log,
                     Progressbar,
                 ),
             )
             results.append(result)
```

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/nbia_cli.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/nbia_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 done_event = threading.Event()
 query: str
 output: io.TextIOWrapper | None = None
 
 
 def version():
-    f = """
+    f = r"""
         _   ______  _______  ______            ____   _ __
        / | / / __ )/  _/   |/_  __/___  ____  / / /__(_) /_
       /  |/ / __  |/ // /| | / / / __ \/ __ \/ / //_/ / __/
      / /|  / /_/ // // ___ |/ / / /_/ / /_/ / / ,< / / /_
     /_/ |_/_____/___/_/  |_/_/  \____/\____/_/_/|_/_/\__/
     """
     print(f)
```

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/utils/conv_response_list.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/utils/conv_response_list.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/utils/md5.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/utils/md5.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/utils/nbia_endpoints.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/utils/nbia_endpoints.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/src/nbiatoolkit/utils/parsers.py` & `nbiatoolkit-1.2.0/src/nbiatoolkit/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nbiatoolkit-1.0.1/PKG-INFO` & `nbiatoolkit-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nbiatoolkit
-Version: 1.0.1
+Version: 1.2.0
 Summary: A python package to query the National Biomedical Imaging Archive (NBIA) database.
 License: MIT
 Author: Jermiah Joseph
-Requires-Python: >=3.10
+Requires-Python: >=3.09
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: cryptography (>=42.0.2,<43.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
@@ -33,19 +34,19 @@
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/jjjermiah/nbia-toolkit)
 [![PyPI version](https://badge.fury.io/py/nbiatoolkit.svg)](https://badge.fury.io/py/nbiatoolkit)
 [![Downloads](https://static.pepy.tech/badge/nbiatoolkit)](https://pepy.tech/project/nbiatoolkit)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/nbiatoolkit.svg?label=pypi%20downloads)](https://pypi.org/project/nbiatoolkit/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/jjjermiah/nbia-toolkit)
 [![Docker Pulls](https://img.shields.io/docker/pulls/jjjermiah/nbiatoolkit)](https://hub.docker.com/r/jjjermiah/nbiatoolkit)
 
-![GitHub milestone details](https://img.shields.io/github/milestones/progress-percent/jjjermiah/nbia-toolkit/1?style=flat-square&label=1.0.0%20Stable%20Release%20Milestone&link=https%3A%2F%2Fgithub.com%2Fjjjermiah%2Fnbia-toolkit%2Fmilestone%2F1)![GitHub milestone details](https://img.shields.io/github/milestones/progress/jjjermiah/nbia-toolkit/1?style=flat-square&label=%20&link=https%3A%2F%2Fgithub.com%2Fjjjermiah%2Fnbia-toolkit%2Fmilestone%2F1)
 [![GitHub issues](https://img.shields.io/github/issues/jjjermiah/nbia-toolkit)](https://github.com/jjjermiah/nbia-toolkit/issues)
 ![GitHub last commit](https://img.shields.io/github/last-commit/jjjermiah/nbia-toolkit)
 
 ## Table of Contents
+
 - [Features](#features)
 - [Installation](#installation)
 - [Python Usage](#python-usage)
 - [CLI Usage](#cli-usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [User Agreements and Disclaimers](#user-agreements-and-disclaimers)
@@ -60,15 +61,15 @@
   - Custom `OAuth2` class for **NBIA**, **TCIA**, including special handling for dedicated server for the **NLST** collection.
 
 - ***Query NBIA database*** for metadata on ***collections***, ***patients***, ***studies***, ***series***, and ***images***
 - Download images from NBIA
   - ***Validate doownloads with MD5 checksums*** for downloaded images
   - **Auto-sort** DICOM files using a user-defined pattern of DICOM tags with specialized ***DICOMSorter class***
 
-![SequenceDiagram](https://www.mermaidchart.com/raw/ce7f489f-bf58-4827-aedb-e379ed7bffd3?theme=dark&version=v0.1&format=svg)
+See [Developer Notes](devnotes/README.md) for more details on the features and the development process.
 
 ## Installation
 
 > [!WARNING]
 > `nbiatoolkit` is currently under development and is not guaranteed to be stable.
 
 It is made available via PyPI and can be installed using pip:
@@ -111,15 +112,15 @@
 
         _   ______  _______  ______            ____   _ __
        / | / / __ )/  _/   |/_  __/___  ____  / / /__(_) /_
       /  |/ / __  |/ // /| | / / / __ \/ __ \/ / //_/ / __/
      / /|  / /_/ // // ___ |/ / / /_/ / /_/ / / ,< / / /_
     /_/ |_/_____/___/_/  |_/_/  \____/\____/_/_/|_/_/\__/
 
-Version: 1.0.0
+Version: 1.0.1
 
 Available CLI tools:
 
 getCollections [-h] [-u USERNAME] [-pw PASSWORD] [-p PREFIX]
                [-o OUTPUTFILE] [--version]
 
 getBodyPartCounts [-h] [-u USERNAME] [-pw PASSWORD] [-c COLLECTION]
```

