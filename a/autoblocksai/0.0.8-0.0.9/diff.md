# Comparing `tmp/autoblocksai-0.0.8.tar.gz` & `tmp/autoblocksai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoblocksai-0.0.8.tar", max compression
+gzip compressed data, was "autoblocksai-0.0.9.tar", max compression
```

## Comparing `autoblocksai-0.0.8.tar` & `autoblocksai-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/LICENSE
--rw-r--r--   0        0        0      969 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/__init__.py
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/__init__.py
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/api/__init__.py
--rw-r--r--   0        0        0     3281 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/api/client.py
--rw-r--r--   0        0        0     1577 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/api/models.py
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/config/__init__.py
--rw-r--r--   0        0        0      101 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/config/constants.py
--rw-r--r--   0        0        0     3666 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/tracer.py
--rw-r--r--   0        0        0     8486 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/util.py
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/vendor/langchain/__init__.py
--rw-r--r--   0        0        0    11550 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/_impl/vendor/langchain/callback.py
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/api/__init__.py
--rw-r--r--   0        0        0       74 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/api/client.py
--rw-r--r--   0        0        0      749 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/api/models.py
--rw-r--r--   0        0        0       67 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/tracer/__init__.py
--rw-r--r--   0        0        0       68 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/tracer/models.py
--rw-r--r--   0        0        0        0 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/vendor/__init__.py
--rw-r--r--   0        0        0       95 2023-09-04 21:57:47.843872 autoblocksai-0.0.8/autoblocks/vendor/langchain.py
--rw-r--r--   0        0        0      793 2023-09-04 21:58:13.432367 autoblocksai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 autoblocksai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/LICENSE
+-rw-r--r--   0        0        0      969 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/api/__init__.py
+-rw-r--r--   0        0        0     3281 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/api/client.py
+-rw-r--r--   0        0        0     1577 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/api/models.py
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/config/__init__.py
+-rw-r--r--   0        0        0      101 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/config/constants.py
+-rw-r--r--   0        0        0     3666 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/tracer.py
+-rw-r--r--   0        0        0     8659 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/util.py
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/vendor/langchain/__init__.py
+-rw-r--r--   0        0        0    11550 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/_impl/vendor/langchain/callback.py
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/api/__init__.py
+-rw-r--r--   0        0        0       74 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/api/client.py
+-rw-r--r--   0        0        0      749 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/api/models.py
+-rw-r--r--   0        0        0       67 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/tracer/__init__.py
+-rw-r--r--   0        0        0       68 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/tracer/models.py
+-rw-r--r--   0        0        0        0 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/vendor/__init__.py
+-rw-r--r--   0        0        0       95 2023-10-10 15:35:16.464666 autoblocksai-0.0.9/autoblocks/vendor/langchain.py
+-rw-r--r--   0        0        0      860 2023-10-10 15:35:38.772977 autoblocksai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 autoblocksai-0.0.9/PKG-INFO
```

### Comparing `autoblocksai-0.0.8/LICENSE` & `autoblocksai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autoblocksai-0.0.8/README.md` & `autoblocksai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `autoblocksai-0.0.8/autoblocks/_impl/api/client.py` & `autoblocksai-0.0.9/autoblocks/_impl/api/client.py`

 * *Files identical despite different names*

### Comparing `autoblocksai-0.0.8/autoblocks/_impl/api/models.py` & `autoblocksai-0.0.9/autoblocks/_impl/api/models.py`

 * *Files identical despite different names*

### Comparing `autoblocksai-0.0.8/autoblocks/_impl/tracer.py` & `autoblocksai-0.0.9/autoblocks/_impl/tracer.py`

 * *Files identical despite different names*

### Comparing `autoblocksai-0.0.8/autoblocks/_impl/util.py` & `autoblocksai-0.0.9/autoblocks/_impl/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,29 +94,36 @@
             "rev-parse",
             "--abbrev-ref",
             "HEAD",
         ]
     )
 
 
+def parse_repo_name_from_origin_url(url: str) -> str:
+    """
+    Parses the org and repo name from the origin URL.
+
+    Examples:
+
+    https://github.com/autoblocksai/javascript-sdk.git -> autoblocksai/javascript-sdk
+    git@gitlab.com:gitlab-com/www-gitlab-com.git -> gitlab-com/www-gitlab-com
+    """
+    return "/".join(url.replace(".git", "").split(":")[1].split("/")[-2:])
+
+
 def get_local_repo_name() -> str:
     url = run_command(
         [
             "git",
             "remote",
             "get-url",
             "origin",
         ]
     )
-    # Parses the owner/repo string out of the remote URL
-    # Eg. https://github.com/autoblocksai/python-sdk.git -> autoblocksai/python-sdk
-    parts = url.split("/")[-2:]
-    owner, repo = parts
-    repo = repo.split(".")[0]
-    return f"{owner}/{repo}"
+    return parse_repo_name_from_origin_url(url)
 
 
 def get_local_commit_data(sha: Optional[str]) -> Commit:
     commit_message_key = "commit_message"
 
     log_format = "%n".join(
         [
```

### Comparing `autoblocksai-0.0.8/autoblocks/_impl/vendor/langchain/callback.py` & `autoblocksai-0.0.9/autoblocks/_impl/vendor/langchain/callback.py`

 * *Files identical despite different names*

### Comparing `autoblocksai-0.0.8/autoblocks/api/models.py` & `autoblocksai-0.0.9/autoblocks/api/models.py`

 * *Files identical despite different names*

### Comparing `autoblocksai-0.0.8/pyproject.toml` & `autoblocksai-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "autoblocksai"
 # The version is not maintained here. It's set in the release workflow via the version input.
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Autoblocks Engineering <engineering@autoblocks.ai>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "autoblocks"}]
 
 [tool.poetry.dependencies]
@@ -31,7 +31,12 @@
 [tool.ruff]
 select = ["E", "F", "I001"]
 line-length = 120
 
 [tool.ruff.isort]
 force-single-line = true
 known-first-party = ["autoblocks"]
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests/autoblocks",
+]
```

### Comparing `autoblocksai-0.0.8/PKG-INFO` & `autoblocksai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoblocksai
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 License: MIT
 Author: Autoblocks Engineering
 Author-email: engineering@autoblocks.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoblocksai Version: 0.0.8 Summary: License: MIT
+Metadata-Version: 2.1 Name: autoblocksai Version: 0.0.9 Summary: License: MIT
 Author: Autoblocks Engineering Author-email: engineering@autoblocks.ai
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
 (>=0.24.0,<0.25.0) Description-Content-Type: text/markdown
                   [https://app.autoblocks.ai/images/logo.png]
```

