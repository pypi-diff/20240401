# Comparing `tmp/encapsia_cli-0.5.8.tar.gz` & `tmp/encapsia_cli-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsia_cli-0.5.8.tar", max compression
+gzip compressed data, was "encapsia_cli-0.5.9.tar", max compression
```

## Comparing `encapsia_cli-0.5.8.tar` & `encapsia_cli-0.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1078 2022-01-07 06:44:24.119730 encapsia_cli-0.5.8/LICENSE
--rw-r--r--   0        0        0     1515 2023-04-24 06:40:03.716923 encapsia_cli-0.5.8/README.md
--rw-r--r--   0        0        0       90 2024-01-26 11:50:55.570510 encapsia_cli-0.5.8/encapsia_cli/__init__.py
--rw-r--r--   0        0        0     1495 2022-01-07 06:44:24.119730 encapsia_cli-0.5.8/encapsia_cli/completion.py
--rw-r--r--   0        0        0     1930 2023-04-24 06:27:52.898295 encapsia_cli-0.5.8/encapsia_cli/config.py
--rw-r--r--   0        0        0     1928 2023-04-24 06:49:10.547106 encapsia_cli-0.5.8/encapsia_cli/database.py
--rw-r--r--   0        0        0     4224 2023-04-24 06:27:52.898295 encapsia_cli-0.5.8/encapsia_cli/encapsia.py
--rw-r--r--   0        0        0     2377 2023-04-24 06:49:28.555269 encapsia_cli-0.5.8/encapsia_cli/fixtures.py
--rw-r--r--   0        0        0     1145 2022-01-07 06:44:24.123731 encapsia_cli-0.5.8/encapsia_cli/help.py
--rw-r--r--   0        0        0      564 2022-01-07 06:44:24.123731 encapsia_cli-0.5.8/encapsia_cli/httpie.py
--rw-r--r--   0        0        0     8320 2023-04-24 06:27:52.898295 encapsia_cli-0.5.8/encapsia_cli/lib.py
--rw-r--r--   0        0        0    18109 2024-01-26 11:47:25.721235 encapsia_cli-0.5.8/encapsia_cli/plugininfo.py
--rw-r--r--   0        0        0    32068 2024-01-26 11:45:53.208673 encapsia_cli-0.5.8/encapsia_cli/plugins.py
--rw-r--r--   0        0        0     4296 2022-01-07 06:44:24.123731 encapsia_cli-0.5.8/encapsia_cli/run.py
--rw-r--r--   0        0        0     1156 2022-01-07 06:44:24.123731 encapsia_cli-0.5.8/encapsia_cli/s3.py
--rw-r--r--   0        0        0     2218 2022-01-07 06:44:24.123731 encapsia_cli-0.5.8/encapsia_cli/schedule.py
--rw-r--r--   0        0        0      520 2022-01-07 06:44:24.123731 encapsia_cli-0.5.8/encapsia_cli/shell.py
--rw-r--r--   0        0        0     3749 2023-02-02 13:22:51.981788 encapsia_cli-0.5.8/encapsia_cli/token.py
--rw-r--r--   0        0        0     4391 2023-04-24 06:27:52.898295 encapsia_cli-0.5.8/encapsia_cli/users.py
--rw-r--r--   0        0        0      495 2024-01-26 11:45:53.208673 encapsia_cli-0.5.8/encapsia_cli/version.py
--rw-r--r--   0        0        0     1575 2024-01-26 12:01:24.870337 encapsia_cli-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 encapsia_cli-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-01-07 06:44:24.119730 encapsia_cli-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1515 2023-04-24 06:40:03.716923 encapsia_cli-0.5.9/README.md
+-rw-r--r--   0        0        0       90 2024-04-01 08:33:14.147826 encapsia_cli-0.5.9/encapsia_cli/__init__.py
+-rw-r--r--   0        0        0     1495 2022-01-07 06:44:24.119730 encapsia_cli-0.5.9/encapsia_cli/completion.py
+-rw-r--r--   0        0        0     1930 2023-04-24 06:27:52.898295 encapsia_cli-0.5.9/encapsia_cli/config.py
+-rw-r--r--   0        0        0     1928 2023-04-24 06:49:10.547106 encapsia_cli-0.5.9/encapsia_cli/database.py
+-rw-r--r--   0        0        0     4224 2023-04-24 06:27:52.898295 encapsia_cli-0.5.9/encapsia_cli/encapsia.py
+-rw-r--r--   0        0        0     2377 2023-04-24 06:49:28.555269 encapsia_cli-0.5.9/encapsia_cli/fixtures.py
+-rw-r--r--   0        0        0     1145 2022-01-07 06:44:24.123731 encapsia_cli-0.5.9/encapsia_cli/help.py
+-rw-r--r--   0        0        0      564 2022-01-07 06:44:24.123731 encapsia_cli-0.5.9/encapsia_cli/httpie.py
+-rw-r--r--   0        0        0     8320 2023-04-24 06:27:52.898295 encapsia_cli-0.5.9/encapsia_cli/lib.py
+-rw-r--r--   0        0        0    18109 2024-01-26 11:47:25.721235 encapsia_cli-0.5.9/encapsia_cli/plugininfo.py
+-rw-r--r--   0        0        0    32068 2024-01-26 11:45:53.208673 encapsia_cli-0.5.9/encapsia_cli/plugins.py
+-rw-r--r--   0        0        0     4296 2022-01-07 06:44:24.123731 encapsia_cli-0.5.9/encapsia_cli/run.py
+-rw-r--r--   0        0        0     1156 2022-01-07 06:44:24.123731 encapsia_cli-0.5.9/encapsia_cli/s3.py
+-rw-r--r--   0        0        0     2218 2022-01-07 06:44:24.123731 encapsia_cli-0.5.9/encapsia_cli/schedule.py
+-rw-r--r--   0        0        0      520 2022-01-07 06:44:24.123731 encapsia_cli-0.5.9/encapsia_cli/shell.py
+-rw-r--r--   0        0        0     3749 2023-02-02 13:22:51.981788 encapsia_cli-0.5.9/encapsia_cli/token.py
+-rw-r--r--   0        0        0     4391 2023-04-24 06:27:52.898295 encapsia_cli-0.5.9/encapsia_cli/users.py
+-rw-r--r--   0        0        0      487 2024-04-01 08:59:42.558421 encapsia_cli-0.5.9/encapsia_cli/version.py
+-rw-r--r--   0        0        0     1575 2024-04-01 08:33:23.219882 encapsia_cli-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 encapsia_cli-0.5.9/PKG-INFO
```

### Comparing `encapsia_cli-0.5.8/LICENSE` & `encapsia_cli-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/README.md` & `encapsia_cli-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/completion.py` & `encapsia_cli-0.5.9/encapsia_cli/completion.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/config.py` & `encapsia_cli-0.5.9/encapsia_cli/config.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/database.py` & `encapsia_cli-0.5.9/encapsia_cli/database.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/encapsia.py` & `encapsia_cli-0.5.9/encapsia_cli/encapsia.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/fixtures.py` & `encapsia_cli-0.5.9/encapsia_cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/help.py` & `encapsia_cli-0.5.9/encapsia_cli/help.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/httpie.py` & `encapsia_cli-0.5.9/encapsia_cli/httpie.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/lib.py` & `encapsia_cli-0.5.9/encapsia_cli/lib.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/plugininfo.py` & `encapsia_cli-0.5.9/encapsia_cli/plugininfo.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/plugins.py` & `encapsia_cli-0.5.9/encapsia_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/run.py` & `encapsia_cli-0.5.9/encapsia_cli/run.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/s3.py` & `encapsia_cli-0.5.9/encapsia_cli/s3.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/schedule.py` & `encapsia_cli-0.5.9/encapsia_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/shell.py` & `encapsia_cli-0.5.9/encapsia_cli/shell.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/token.py` & `encapsia_cli-0.5.9/encapsia_cli/token.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/encapsia_cli/users.py` & `encapsia_cli-0.5.9/encapsia_cli/users.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.8/pyproject.toml` & `encapsia_cli-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encapsia-cli"
-version = "0.5.8"
+version = "0.5.9"
 description = "Client CLI for talking to an Encapsia system."
 readme = "README.md"
 authors = ["Timothy Corbett-Clark <timothy.corbettclark@gmail.com>"]
 maintainers = ["Petre Mierluțiu <pmierlutiu@cmedtechnology.com>"]
 license = "MIT"
 keywords = ["encapsia", "eSource", "EDC", "Clinical Trials"]
 homepage = "https://github.com/Encapsia/encapsia-cli"
```

### Comparing `encapsia_cli-0.5.8/PKG-INFO` & `encapsia_cli-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsia-cli
-Version: 0.5.8
+Version: 0.5.9
 Summary: Client CLI for talking to an Encapsia system.
 Home-page: https://github.com/Encapsia/encapsia-cli
 License: MIT
 Keywords: encapsia,eSource,EDC,Clinical Trials
 Author: Timothy Corbett-Clark
 Author-email: timothy.corbettclark@gmail.com
 Maintainer: Petre Mierluțiu
```

