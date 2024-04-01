# Comparing `tmp/bits_github-1.4.0.tar.gz` & `tmp/bits_github-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits_github-1.4.0.tar", max compression
+gzip compressed data, was "bits_github-1.4.1.tar", max compression
```

## Comparing `bits_github-1.4.0.tar` & `bits_github-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       45 2024-04-01 17:50:32.484241 bits_github-1.4.0/README.md
--rw-r--r--   0        0        0       65 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/__init__.py
--rw-r--r--   0        0        0    25745 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/app.py
--rw-r--r--   0        0        0    13646 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/auditlogs.py
--rw-r--r--   0        0        0    16434 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/client.py
--rw-r--r--   0        0        0     1899 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/datastore.py
--rw-r--r--   0        0        0    10143 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/firestore.py
--rw-r--r--   0        0        0     6904 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/helpers.py
--rw-r--r--   0        0        0     2719 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/sync.py
--rw-r--r--   0        0        0    24647 2024-04-01 17:50:32.484241 bits_github-1.4.0/bits/github/update.py
--rw-r--r--   0        0        0     1207 2024-04-01 17:50:32.488241 bits_github-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 bits_github-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-01 18:45:25.965250 bits_github-1.4.1/README.md
+-rw-r--r--   0        0        0       65 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/__init__.py
+-rw-r--r--   0        0        0    25745 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/app.py
+-rw-r--r--   0        0        0    13646 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/auditlogs.py
+-rw-r--r--   0        0        0    16434 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/client.py
+-rw-r--r--   0        0        0     1899 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/datastore.py
+-rw-r--r--   0        0        0    10143 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/firestore.py
+-rw-r--r--   0        0        0     6904 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/helpers.py
+-rw-r--r--   0        0        0     2719 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/sync.py
+-rw-r--r--   0        0        0    24647 2024-04-01 18:45:25.965250 bits_github-1.4.1/bits/github/update.py
+-rw-r--r--   0        0        0     1201 2024-04-01 18:45:25.965250 bits_github-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 bits_github-1.4.1/PKG-INFO
```

### Comparing `bits_github-1.4.0/bits/github/__init__.py` & `bits_github-1.4.1/bits/github/__init__.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/app.py` & `bits_github-1.4.1/bits/github/app.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/auditlogs.py` & `bits_github-1.4.1/bits/github/auditlogs.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/client.py` & `bits_github-1.4.1/bits/github/client.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/datastore.py` & `bits_github-1.4.1/bits/github/datastore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/firestore.py` & `bits_github-1.4.1/bits/github/firestore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/helpers.py` & `bits_github-1.4.1/bits/github/helpers.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/sync.py` & `bits_github-1.4.1/bits/github/sync.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/bits/github/update.py` & `bits_github-1.4.1/bits/github/update.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.0/pyproject.toml` & `bits_github-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 license = "BSD-3-Clause"
 name = "bits-github"
 packages = [
     { include = "bits" },
 ]
 readme = "README.md"
 repository = "https://github.com/broadinstitute/bits-github.git"
-version = "1.4.0"
+version = "1.4.1"
 
 [tool.poetry.dependencies]
 python = "^3.9"  # Compatible python versions must be declared here
 
 bits-google = "^1.13.8"
 google-cloud-datastore = "^2.19.0"
 google-cloud-firestore = "^2.15.0"
 python-dateutil = "^2.9.0.post0"
-pytz = "^2024.1"
+pytz = "*"
 testtools = "^2.7.1"
 twine = "^5.0.0"
 wheel = "^0.43.0"
 
 [tool.ruff]
 line-length = 120
```

### Comparing `bits_github-1.4.0/PKG-INFO` & `bits_github-1.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bits-github
-Version: 1.4.0
+Version: 1.4.1
 Summary: BITS GitHub Package for Python
 Home-page: https://github.com/broadinstitute/bits-github.git
 License: BSD-3-Clause
 Keywords: bits,github
 Author: Lukas Karlsson
 Author-email: karlsson@broadinstitute.org
 Requires-Python: >=3.9,<4.0
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bits-google (>=1.13.8,<2.0.0)
 Requires-Dist: google-cloud-datastore (>=2.19.0,<3.0.0)
 Requires-Dist: google-cloud-firestore (>=2.15.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
-Requires-Dist: pytz (>=2024.1,<2025.0)
+Requires-Dist: pytz
 Requires-Dist: testtools (>=2.7.1,<3.0.0)
 Requires-Dist: twine (>=5.0.0,<6.0.0)
 Requires-Dist: wheel (>=0.43.0,<0.44.0)
 Project-URL: Repository, https://github.com/broadinstitute/bits-github.git
 Description-Content-Type: text/markdown
 
 # bits-github
```

