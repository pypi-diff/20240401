# Comparing `tmp/jf-ingest-0.0.8.tar.gz` & `tmp/jf-ingest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jf-ingest-0.0.8.tar", last modified: Tue Oct 10 20:34:04 2023, max compression
+gzip compressed data, was "jf-ingest-0.0.9.tar", last modified: Mon Oct 16 19:49:45 2023, max compression
```

## Comparing `jf-ingest-0.0.8.tar` & `jf-ingest-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     2772 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1066 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      399 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       19 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/jf_ingest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/jf_ingest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/jf_ingest/jf_git/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/jf_ingest/jf_git/__init__.py
--rw-r--r--   0 root         (0) root         (0)      217 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/jf_ingest/jf_git/standardized_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/jf_ingest/jf_jira/
--rw-r--r--   0 root         (0) root         (0)    10267 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/jf_ingest/jf_jira/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4351 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/jf_ingest/jf_jira/downloaders.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/jf_ingest/logger.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/jf_ingest/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/jf_ingest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      399 2023-10-10 20:34:04.000000 jf-ingest-0.0.8/jf_ingest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      553 2023-10-10 20:34:04.000000 jf-ingest-0.0.8/jf_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-10 20:34:04.000000 jf-ingest-0.0.8/jf_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-10 20:34:04.000000 jf-ingest-0.0.8/jf_ingest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-10-10 20:34:04.000000 jf-ingest-0.0.8/jf_ingest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    34029 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/pdm.lock
--rw-r--r--   0 root         (0) root         (0)      830 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/tests/jf_jira/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/tests/jf_jira/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 20:34:04.557619 jf-ingest-0.0.8/tests/jf_jira/fixtures/
--rw-r--r--   0 root         (0) root         (0)     1837 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/tests/jf_jira/fixtures/jira_fields_response.json
--rw-r--r--   0 root         (0) root         (0)     4246 2023-10-10 20:33:34.000000 jf-ingest-0.0.8/tests/jf_jira/test_jira_downloaders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      427 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       19 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.716625 jf-ingest-0.0.9/jf_ingest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/jf_ingest/jf_git/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_git/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      217 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_git/standardized_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/jf_ingest/jf_jira/
+-rw-r--r--   0 root         (0) root         (0)    10290 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_jira/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_jira/auth.py
+-rw-r--r--   0 root         (0) root         (0)     3217 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_jira/downloaders.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/jf_ingest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      427 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      611 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    34489 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/pdm.lock
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/tests/jf_jira/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/tests/jf_jira/fixtures/
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/fixtures/jira_fields_response.json
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/test_jira_auth.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/test_jira_downloaders.py
```

### Comparing `jf-ingest-0.0.8/.gitignore` & `jf-ingest-0.0.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 var/
 wheels/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+._version.py
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `jf-ingest-0.0.8/LICENSE` & `jf-ingest-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jf-ingest-0.0.8/jf_ingest/jf_jira/__init__.py` & `jf-ingest-0.0.9/jf_ingest/jf_jira/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import chain
 import traceback
+from jf_ingest.jf_jira.auth import JiraAuthConfig, get_jira_connection, JiraAuthMethod
 from jf_ingest.jf_jira.downloaders import (
     IssueMetadata,
     detect_issues_needing_re_download,
     detect_issues_needing_sync,
     download_all_issue_metadata,
     download_boards_and_sprints,
     download_customfieldoptions,
@@ -26,23 +27,21 @@
 from jf_ingest.utils import IngestIOHelper
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class JiraIngestionConfig:
-    # IO information
     s3_bucket: str
     s3_path: str
     local_file_path: str
+    company_slug: str
 
-    # Jira Server info
-    gdpr_active: bool
-    required_email_domains: bool
-    is_email_required: bool
+    # Jira Auth Info
+    auth_config: JiraAuthConfig
 
     # Fields information
     # NOTE: I assumed these are all strs
     include_fields: list[str]
     exclude_fields: list[str]
 
     # Projects information
@@ -91,16 +90,16 @@
     try:
         # For JF Ingest logic, logger should always be set at debug!
         # This is for better log management when deal with agent,
         # where we sometimes want to hide stack traces from clients,
         # but also NOT upload their sensitive information
         original_log_level = logger.level
         logger.setLevel(level=logging.DEBUG)
-        # TODO: Set up logic to fetch jira connection!
-        jira_connection = None
+
+        jira_connection = get_jira_connection(config=config.auth_config)
 
         ingest_io_helper = IngestIOHelper(
             s3_bucket=config.s3_bucket,
             s3_path=config.s3_path,
             local_file_path=f"{config.local_file_path}/jira",
         )
```

### Comparing `jf-ingest-0.0.8/jf_ingest.egg-info/SOURCES.txt` & `jf-ingest-0.0.9/jf_ingest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,12 +11,14 @@
 jf_ingest.egg-info/SOURCES.txt
 jf_ingest.egg-info/dependency_links.txt
 jf_ingest.egg-info/requires.txt
 jf_ingest.egg-info/top_level.txt
 jf_ingest/jf_git/__init__.py
 jf_ingest/jf_git/standardized_models.py
 jf_ingest/jf_jira/__init__.py
+jf_ingest/jf_jira/auth.py
 jf_ingest/jf_jira/downloaders.py
 tests/__init__.py
 tests/jf_jira/__init__.py
+tests/jf_jira/test_jira_auth.py
 tests/jf_jira/test_jira_downloaders.py
 tests/jf_jira/fixtures/jira_fields_response.json
```

### Comparing `jf-ingest-0.0.8/pdm.lock` & `jf-ingest-0.0.9/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "dev"]
 cross_platform = true
 static_urls = false
 lock_version = "4.3"
-content_hash = "sha256:16d96e2fdffcceb5de6e23293a9fee733b49395244772875df389f6f01307b0f"
+content_hash = "sha256:2f1532130a58913a5b32d20b4fc43c9469d06c40072fcfba077b049aa8400266"
 
 [[package]]
 name = "bleach"
 version = "6.0.0"
 requires_python = ">=3.7"
 summary = "An easy safelist-based HTML-sanitizing tool."
 dependencies = [
@@ -20,26 +20,26 @@
 files = [
     {file = "bleach-6.0.0-py3-none-any.whl", hash = "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"},
     {file = "bleach-6.0.0.tar.gz", hash = "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414"},
 ]
 
 [[package]]
 name = "build"
-version = "0.10.0"
+version = "1.0.3"
 requires_python = ">= 3.7"
 summary = "A simple, correct Python build frontend"
 dependencies = [
     "colorama; os_name == \"nt\"",
     "packaging>=19.0",
     "pyproject-hooks",
     "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 files = [
-    {file = "build-0.10.0-py3-none-any.whl", hash = "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171"},
-    {file = "build-0.10.0.tar.gz", hash = "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"},
+    {file = "build-1.0.3-py3-none-any.whl", hash = "sha256:589bf99a67df7c9cf07ec0ac0e5e2ea5d4b37ac63301c4986d1acb126aa83f8f"},
+    {file = "build-1.0.3.tar.gz", hash = "sha256:538aab1b64f9828977f84bc63ae570b060a8ed1be419e7870b8b4fc5e6ea553b"},
 ]
 
 [[package]]
 name = "certifi"
 version = "2023.7.22"
 requires_python = ">=3.6"
 summary = "Python package for providing Mozilla's CA Bundle."
@@ -443,14 +443,27 @@
 ]
 files = [
     {file = "pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
     {file = "pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 
 [[package]]
+name = "pytest-mock"
+version = "3.11.1"
+requires_python = ">=3.7"
+summary = "Thin-wrapper around the mock package for easier use with pytest"
+dependencies = [
+    "pytest>=5.0",
+]
+files = [
+    {file = "pytest-mock-3.11.1.tar.gz", hash = "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"},
+    {file = "pytest_mock-3.11.1-py3-none-any.whl", hash = "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39"},
+]
+
+[[package]]
 name = "pywin32-ctypes"
 version = "0.2.2"
 requires_python = ">=3.6"
 summary = "A (partial) reimplementation of pywin32 using ctypes/cffi"
 files = [
     {file = "pywin32-ctypes-0.2.2.tar.gz", hash = "sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60"},
     {file = "pywin32_ctypes-0.2.2-py3-none-any.whl", hash = "sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7"},
```

### Comparing `jf-ingest-0.0.8/pyproject.toml` & `jf-ingest-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,43 @@
 description = "library used for ingesting jira data"
 authors = [
     {name = "jellyfish-oss", email = "oss@jellyfish.co"},
 ]
 dependencies = [
     "jira >= 2.0.0, < 2.1",
     "requests-mock==1.11.0",
+    "build>=1.0.3",
 ]
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 [project.urls]
 "Homepage" = "https://github.com/Jellyfish-AI/jf_ingest"
 
+
 [tool.pdm]
 [[tool.pdm.source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [tool.pdm.build]
 excludes = ["**/.pytest_cache/**"]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.4.0",
-    "build>=0.10.0", 
     "twine>=4.0.2",
     "setuptools-scm>=7.1.0",
+    "pytest-mock>=3.11.1",
+    "build>=1.0.3",
 ]
 
+# To stop pdm add and pdm lock from yeeting this [tool.setuptools_scm] tag,
+# we must specify a version_file
+[tool.setuptools_scm]
+version_file = "._version.py"
 
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel", "setuptools_scm[toml]>=6.0",]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools_scm]
```

### Comparing `jf-ingest-0.0.8/tests/jf_jira/fixtures/jira_fields_response.json` & `jf-ingest-0.0.9/tests/jf_jira/fixtures/jira_fields_response.json`

 * *Files identical despite different names*

### Comparing `jf-ingest-0.0.8/tests/jf_jira/test_jira_downloaders.py` & `jf-ingest-0.0.9/tests/jf_jira/test_jira_downloaders.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 import os
 
 import requests_mock
 from unittest import TestCase
 
-from jf_ingest.jf_jira.downloaders import get_jira_connection, download_fields
+from jf_ingest.jf_jira.auth import JiraAuthConfig, get_jira_connection
+from jf_ingest.jf_jira.downloaders import download_fields
 
 MOCK_SERVER_INFO_RESP = (
     '{"baseUrl":"https://test-co.atlassian.net","version":"1001.0.0-SNAPSHOT",'
     '"versionNumbers":[1001,0,0],"deploymentType":"Cloud","buildNumber":100218,'
     '"buildDate":"2023-03-16T08:21:48.000-0400","serverTime":"2023-03-17T16:32:45.255-0400",'
     '"scmInfo":"9999999999999999999999999999999999999999","serverTitle":"JIRA",'
     '"defaultLocale":{"locale":"en_US"}} '
 )
 
 
 def get_connection(mocker: requests_mock.Mocker):
-    class PartialConfig:
-        jira_url = "https://test-co.atlassian.net/"
-        skip_ssl_verification = False
-
-    class PartialCreds:
-        jira_password = None
-        jira_username = None
-        jira_bearer_token = "asdf"
 
-    config = PartialConfig()
-    creds = PartialCreds()
+    auth_config = JiraAuthConfig(
+        url="https://test-co.atlassian.net/",
+        personal_access_token="asdf",
+        company_slug="test_co",
+    )
     # you can test behavior against a live jira instance by setting an email as `jira_username`
     # and storing a generated token in env and retrieving like so:
     # creds.jira_bearer_token = os.environ.get('JIRA_TOKEN')
 
     # https://test-co.atlassian.net/rest/api/2/serverInfo
     mocker.register_uri(
         "GET",
         "https://test-co.atlassian.net/rest/api/2/serverInfo",
         text=f"{MOCK_SERVER_INFO_RESP}",
     )
-    jira_conn = get_jira_connection(config, creds, max_retries=1)
+    jira_conn = get_jira_connection(config=auth_config, max_retries=1)
 
     return jira_conn
 
 
 class TestJiraDownload(TestCase):
     URL_BASE = "https://test-co.atlassian.net/rest/api/2/search"
```

