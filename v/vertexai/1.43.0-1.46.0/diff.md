# Comparing `tmp/vertexai-1.43.0.tar.gz` & `tmp/vertexai-1.46.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertexai-1.43.0.tar", last modified: Thu Mar  7 17:53:14 2024, max compression
+gzip compressed data, was "vertexai-1.46.0.tar", last modified: Mon Apr  1 19:53:03 2024, max compression
```

## Comparing `vertexai-1.43.0.tar` & `vertexai-1.46.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-03-07 17:53:13.000000 vertexai-1.43.0/
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    11358 2023-05-05 15:54:43.000000 vertexai-1.43.0/LICENSE
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7585 2024-03-07 17:53:13.000000 vertexai-1.43.0/PKG-INFO
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      264 2024-03-05 18:46:47.000000 vertexai-1.43.0/README.md
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      519 2024-03-06 23:28:55.000000 vertexai-1.43.0/pyproject.toml
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)       38 2024-03-07 17:53:13.000000 vertexai-1.43.0/setup.cfg
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     5856 2024-03-06 23:54:27.000000 vertexai-1.43.0/setup.py
-drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-03-07 17:53:13.000000 vertexai-1.43.0/src/
-drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-03-07 17:53:13.000000 vertexai-1.43.0/src/vertexai.egg-info/
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7585 2024-03-07 17:53:13.000000 vertexai-1.43.0/src/vertexai.egg-info/PKG-INFO
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      255 2024-03-07 17:53:13.000000 vertexai-1.43.0/src/vertexai.egg-info/SOURCES.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-03-07 17:53:13.000000 vertexai-1.43.0/src/vertexai.egg-info/dependency_links.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-03-05 19:23:09.000000 vertexai-1.43.0/src/vertexai.egg-info/not-zip-safe
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     2845 2024-03-07 17:53:13.000000 vertexai-1.43.0/src/vertexai.egg-info/requires.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-03-07 17:53:13.000000 vertexai-1.43.0/src/vertexai.egg-info/top_level.txt
+drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-01 19:53:03.000000 vertexai-1.46.0/
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    11358 2023-05-05 15:54:43.000000 vertexai-1.46.0/LICENSE
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7585 2024-04-01 19:53:03.000000 vertexai-1.46.0/PKG-INFO
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      264 2024-03-07 21:35:24.000000 vertexai-1.46.0/README.md
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      522 2024-04-01 19:52:56.000000 vertexai-1.46.0/pyproject.toml
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)       38 2024-04-01 19:53:03.000000 vertexai-1.46.0/setup.cfg
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     6004 2024-03-14 23:52:24.000000 vertexai-1.46.0/setup.py
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      625 2024-04-01 16:54:21.000000 vertexai-1.46.0/version.py
+drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-01 19:53:03.000000 vertexai-1.46.0/vertexai.egg-info/
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7585 2024-04-01 19:53:03.000000 vertexai-1.46.0/vertexai.egg-info/PKG-INFO
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      242 2024-04-01 19:53:03.000000 vertexai-1.46.0/vertexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-01 19:53:03.000000 vertexai-1.46.0/vertexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-01 19:32:19.000000 vertexai-1.46.0/vertexai.egg-info/not-zip-safe
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     2845 2024-04-01 19:53:03.000000 vertexai-1.46.0/vertexai.egg-info/requires.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        8 2024-04-01 19:53:03.000000 vertexai-1.46.0/vertexai.egg-info/top_level.txt
```

### Comparing `vertexai-1.43.0/LICENSE` & `vertexai-1.46.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vertexai-1.43.0/PKG-INFO` & `vertexai-1.46.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 Metadata-Version: 2.1
 Name: vertexai
-Version: 1.43.0
+Version: 1.46.0
 Summary: Please run pip install google-cloud-aiplatform to use the Vertex SDK.
 Home-page: https://github.com/googleapis/python-aiplatform
 Author: Google LLC
 Author-email: Google LLC <googleapis-packages@google.com>
 License: Apache 2.0
 Project-URL: repository, https://github.com/googleapis/python-aiplatform.git
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: google-cloud-aiplatform>=1.43.0
+Requires-Dist: google-cloud-aiplatform==1.46.0
 Provides-Extra: endpoint
 Requires-Dist: requests>=2.28.1; extra == "endpoint"
 Provides-Extra: full
-Requires-Dist: pydantic<2; extra == "full"
-Requires-Dist: pyyaml==5.3.1; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "full"
-Requires-Dist: google-cloud-logging<4.0; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
 Requires-Dist: requests>=2.28.1; extra == "full"
+Requires-Dist: google-cloud-logging<4.0; extra == "full"
+Requires-Dist: starlette>=0.17.1; extra == "full"
+Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "full"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
+Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "full"
+Requires-Dist: lit-nlp==0.4.0; extra == "full"
+Requires-Dist: google-cloud-bigquery; extra == "full"
 Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "full"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
-Requires-Dist: docker>=5.0.3; extra == "full"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
 Requires-Dist: numpy>=1.15.0; extra == "full"
-Requires-Dist: pyarrow>=6.0.1; extra == "full"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
-Requires-Dist: google-cloud-bigquery-storage; extra == "full"
-Requires-Dist: google-cloud-bigquery; extra == "full"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
-Requires-Dist: starlette>=0.17.1; extra == "full"
-Requires-Dist: google-vizier>=0.1.6; extra == "full"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "full"
 Requires-Dist: cloudpickle<3.0; extra == "full"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: google-vizier>=0.1.6; extra == "full"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
-Requires-Dist: lit-nlp==0.4.0; extra == "full"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
+Requires-Dist: docker>=5.0.3; extra == "full"
 Requires-Dist: pandas>=1.0.0; extra == "full"
+Requires-Dist: pyyaml==5.3.1; extra == "full"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
+Requires-Dist: pyarrow>=6.0.1; extra == "full"
+Requires-Dist: google-cloud-bigquery-storage; extra == "full"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
+Requires-Dist: pydantic<2; extra == "full"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "full"
 Provides-Extra: metadata
 Requires-Dist: pandas>=1.0.0; extra == "metadata"
 Requires-Dist: numpy>=1.15.0; extra == "metadata"
 Provides-Extra: tensorboard
 Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "tensorboard"
 Provides-Extra: testing
-Requires-Dist: pydantic<2; extra == "testing"
-Requires-Dist: pyyaml==5.3.1; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "testing"
-Requires-Dist: google-cloud-logging<4.0; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
 Requires-Dist: requests>=2.28.1; extra == "testing"
+Requires-Dist: google-cloud-logging<4.0; extra == "testing"
+Requires-Dist: starlette>=0.17.1; extra == "testing"
+Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "testing"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
+Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "testing"
+Requires-Dist: lit-nlp==0.4.0; extra == "testing"
+Requires-Dist: google-cloud-bigquery; extra == "testing"
 Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "testing"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
-Requires-Dist: docker>=5.0.3; extra == "testing"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
 Requires-Dist: numpy>=1.15.0; extra == "testing"
-Requires-Dist: pyarrow>=6.0.1; extra == "testing"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
-Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
-Requires-Dist: google-cloud-bigquery; extra == "testing"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
-Requires-Dist: starlette>=0.17.1; extra == "testing"
-Requires-Dist: google-vizier>=0.1.6; extra == "testing"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "testing"
 Requires-Dist: cloudpickle<3.0; extra == "testing"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: google-vizier>=0.1.6; extra == "testing"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
-Requires-Dist: lit-nlp==0.4.0; extra == "testing"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
+Requires-Dist: docker>=5.0.3; extra == "testing"
 Requires-Dist: pandas>=1.0.0; extra == "testing"
+Requires-Dist: pyyaml==5.3.1; extra == "testing"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
+Requires-Dist: pyarrow>=6.0.1; extra == "testing"
+Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
+Requires-Dist: pydantic<2; extra == "testing"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "testing"
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: bigframes; python_version >= "3.10" and extra == "testing"
 Requires-Dist: google-api-core<3.0.0,>=2.11; extra == "testing"
 Requires-Dist: grpcio-testing; extra == "testing"
 Requires-Dist: ipython; extra == "testing"
```

### Comparing `vertexai-1.43.0/pyproject.toml` & `vertexai-1.46.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vertexai"
-version = "1.43.0"
+dynamic = ["version"]
 dependencies = [
-  "google-cloud-aiplatform >= 1.43.0",
+  "google-cloud-aiplatform == 1.46.0",
 ]
 authors = [
   { name="Google LLC", email="googleapis-packages@google.com" },
 ]
 license = {text = "Apache 2.0"}
 description = "Please run pip install google-cloud-aiplatform to use the Vertex SDK."
 readme = "README.md"
```

### Comparing `vertexai-1.43.0/setup.py` & `vertexai-1.46.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 description = "Vertex AI API client library"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 readme_filename = os.path.join(package_root, "README.md")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
+version = {}
+with open(os.path.join(package_root, "version.py")) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
 tensorboard_extra_require = ["tensorflow >=2.3.0, <2.15.0"]
 metadata_extra_require = ["pandas >= 1.0.0", "numpy>=1.15.0"]
 xai_extra_require = ["tensorflow >=2.3.0, <3.0.0dev"]
 lit_extra_require = [
     "tensorflow >= 2.3.0, <3.0.0dev",
     "pandas >= 1.0.0",
     "lit-nlp == 0.4.0",
@@ -132,23 +137,24 @@
         "xgboost_ray",
         "requests-toolbelt < 1.0.0",
     ]
 )
 
 setuptools.setup(
     name=name,
+    version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="vertex-sdk-dev-pypi@google.com",
     license="Apache 2.0",
     url="https://github.com/googleapis/python-aiplatform",
     platforms="Posix; MacOS X; Windows",
     include_package_data=True,
-    install_requires=["google-cloud-aiplatform >= 1.43.0, < 2.0.0dev"],
+    install_requires=[f"google-cloud-aiplatform == {version}"],
     extras_require={
         "endpoint": endpoint_extra_require,
         "full": full_extra_require,
         "metadata": metadata_extra_require,
         "tensorboard": tensorboard_extra_require,
         "testing": testing_extra_require,
         "xai": xai_extra_require,
```

### Comparing `vertexai-1.43.0/src/vertexai.egg-info/PKG-INFO` & `vertexai-1.46.0/vertexai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 Metadata-Version: 2.1
 Name: vertexai
-Version: 1.43.0
+Version: 1.46.0
 Summary: Please run pip install google-cloud-aiplatform to use the Vertex SDK.
 Home-page: https://github.com/googleapis/python-aiplatform
 Author: Google LLC
 Author-email: Google LLC <googleapis-packages@google.com>
 License: Apache 2.0
 Project-URL: repository, https://github.com/googleapis/python-aiplatform.git
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: google-cloud-aiplatform>=1.43.0
+Requires-Dist: google-cloud-aiplatform==1.46.0
 Provides-Extra: endpoint
 Requires-Dist: requests>=2.28.1; extra == "endpoint"
 Provides-Extra: full
-Requires-Dist: pydantic<2; extra == "full"
-Requires-Dist: pyyaml==5.3.1; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "full"
-Requires-Dist: google-cloud-logging<4.0; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
 Requires-Dist: requests>=2.28.1; extra == "full"
+Requires-Dist: google-cloud-logging<4.0; extra == "full"
+Requires-Dist: starlette>=0.17.1; extra == "full"
+Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "full"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
+Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "full"
+Requires-Dist: lit-nlp==0.4.0; extra == "full"
+Requires-Dist: google-cloud-bigquery; extra == "full"
 Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "full"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
-Requires-Dist: docker>=5.0.3; extra == "full"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
 Requires-Dist: numpy>=1.15.0; extra == "full"
-Requires-Dist: pyarrow>=6.0.1; extra == "full"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
-Requires-Dist: google-cloud-bigquery-storage; extra == "full"
-Requires-Dist: google-cloud-bigquery; extra == "full"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
-Requires-Dist: starlette>=0.17.1; extra == "full"
-Requires-Dist: google-vizier>=0.1.6; extra == "full"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "full"
 Requires-Dist: cloudpickle<3.0; extra == "full"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: google-vizier>=0.1.6; extra == "full"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
-Requires-Dist: lit-nlp==0.4.0; extra == "full"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
+Requires-Dist: docker>=5.0.3; extra == "full"
 Requires-Dist: pandas>=1.0.0; extra == "full"
+Requires-Dist: pyyaml==5.3.1; extra == "full"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
+Requires-Dist: pyarrow>=6.0.1; extra == "full"
+Requires-Dist: google-cloud-bigquery-storage; extra == "full"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
+Requires-Dist: pydantic<2; extra == "full"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "full"
 Provides-Extra: metadata
 Requires-Dist: pandas>=1.0.0; extra == "metadata"
 Requires-Dist: numpy>=1.15.0; extra == "metadata"
 Provides-Extra: tensorboard
 Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "tensorboard"
 Provides-Extra: testing
-Requires-Dist: pydantic<2; extra == "testing"
-Requires-Dist: pyyaml==5.3.1; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "testing"
-Requires-Dist: google-cloud-logging<4.0; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
 Requires-Dist: requests>=2.28.1; extra == "testing"
+Requires-Dist: google-cloud-logging<4.0; extra == "testing"
+Requires-Dist: starlette>=0.17.1; extra == "testing"
+Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "testing"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
+Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "testing"
+Requires-Dist: lit-nlp==0.4.0; extra == "testing"
+Requires-Dist: google-cloud-bigquery; extra == "testing"
 Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "testing"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
-Requires-Dist: docker>=5.0.3; extra == "testing"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
 Requires-Dist: numpy>=1.15.0; extra == "testing"
-Requires-Dist: pyarrow>=6.0.1; extra == "testing"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
-Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
-Requires-Dist: google-cloud-bigquery; extra == "testing"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
-Requires-Dist: starlette>=0.17.1; extra == "testing"
-Requires-Dist: google-vizier>=0.1.6; extra == "testing"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "testing"
 Requires-Dist: cloudpickle<3.0; extra == "testing"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: google-vizier>=0.1.6; extra == "testing"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
-Requires-Dist: lit-nlp==0.4.0; extra == "testing"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
+Requires-Dist: docker>=5.0.3; extra == "testing"
 Requires-Dist: pandas>=1.0.0; extra == "testing"
+Requires-Dist: pyyaml==5.3.1; extra == "testing"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
+Requires-Dist: pyarrow>=6.0.1; extra == "testing"
+Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
+Requires-Dist: pydantic<2; extra == "testing"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "testing"
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: bigframes; python_version >= "3.10" and extra == "testing"
 Requires-Dist: google-api-core<3.0.0,>=2.11; extra == "testing"
 Requires-Dist: grpcio-testing; extra == "testing"
 Requires-Dist: ipython; extra == "testing"
```

### Comparing `vertexai-1.43.0/src/vertexai.egg-info/requires.txt` & `vertexai-1.46.0/vertexai.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-google-cloud-aiplatform>=1.43.0
+google-cloud-aiplatform==1.46.0
 
 [autologging]
 mlflow<=2.1.1,>=1.27.0
 
 [cloud_profiler]
 tensorboard-plugin-profile<3.0.0dev,>=2.4.0
 werkzeug<2.1.0dev,>=2.0.0
@@ -16,45 +16,45 @@
 [datasets:python_version >= "3.11"]
 pyarrow>=10.0.1
 
 [endpoint]
 requests>=2.28.1
 
 [full]
-pydantic<2
-pyyaml==5.3.1
-tensorflow<3.0.0dev,>=2.3.0
-fastapi<0.103.1,>=0.71.0
-google-cloud-logging<4.0
 requests>=2.28.1
+google-cloud-logging<4.0
+starlette>=0.17.1
+fastapi<0.103.1,>=0.71.0
+explainable-ai-sdk>=1.0.0
+lit-nlp==0.4.0
+google-cloud-bigquery
 tensorflow<2.15.0,>=2.3.0
-urllib3<1.27,>=1.21.1
-docker>=5.0.3
+pandas<2.2.0,>=1.0.0
+tensorflow<3.0.0dev,>=2.3.0
 numpy>=1.15.0
-pyarrow>=6.0.1
 httpx<0.25.0,>=0.23.0
-google-cloud-bigquery-storage
-google-cloud-bigquery
-explainable-ai-sdk>=1.0.0
-mlflow<=2.1.1,>=1.27.0
-starlette>=0.17.1
-google-vizier>=0.1.6
 cloudpickle<3.0
+google-vizier>=0.1.6
 uvicorn[standard]>=0.16.0
-pandas<2.2.0,>=1.0.0
-lit-nlp==0.4.0
+mlflow<=2.1.1,>=1.27.0
+docker>=5.0.3
 pandas>=1.0.0
+pyyaml==5.3.1
+urllib3<1.27,>=1.21.1
+pyarrow>=6.0.1
+google-cloud-bigquery-storage
+pydantic<2
 
 [full:python_version < "3.11"]
-ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 pyarrow<8.0dev,>=3.0.0
+ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 
 [full:python_version >= "3.11"]
-ray[default]<=2.9.3,>=2.5
 pyarrow>=10.0.1
+ray[default]<=2.9.3,>=2.5
 
 [lit]
 tensorflow<3.0.0dev,>=2.3.0
 pandas>=1.0.0
 lit-nlp==0.4.0
 explainable-ai-sdk>=1.0.0
 
@@ -93,37 +93,37 @@
 [ray:python_version >= "3.11"]
 ray[default]<=2.9.3,>=2.5
 
 [tensorboard]
 tensorflow<2.15.0,>=2.3.0
 
 [testing]
-pydantic<2
-pyyaml==5.3.1
-tensorflow<3.0.0dev,>=2.3.0
-fastapi<0.103.1,>=0.71.0
-google-cloud-logging<4.0
 requests>=2.28.1
+google-cloud-logging<4.0
+starlette>=0.17.1
+fastapi<0.103.1,>=0.71.0
+explainable-ai-sdk>=1.0.0
+lit-nlp==0.4.0
+google-cloud-bigquery
 tensorflow<2.15.0,>=2.3.0
-urllib3<1.27,>=1.21.1
-docker>=5.0.3
+pandas<2.2.0,>=1.0.0
+tensorflow<3.0.0dev,>=2.3.0
 numpy>=1.15.0
-pyarrow>=6.0.1
 httpx<0.25.0,>=0.23.0
-google-cloud-bigquery-storage
-google-cloud-bigquery
-explainable-ai-sdk>=1.0.0
-mlflow<=2.1.1,>=1.27.0
-starlette>=0.17.1
-google-vizier>=0.1.6
 cloudpickle<3.0
+google-vizier>=0.1.6
 uvicorn[standard]>=0.16.0
-pandas<2.2.0,>=1.0.0
-lit-nlp==0.4.0
+mlflow<=2.1.1,>=1.27.0
+docker>=5.0.3
 pandas>=1.0.0
+pyyaml==5.3.1
+urllib3<1.27,>=1.21.1
+pyarrow>=6.0.1
+google-cloud-bigquery-storage
+pydantic<2
 tensorboard-plugin-profile<3.0.0dev,>=2.4.0
 werkzeug<2.1.0dev,>=2.0.0
 tensorflow<3.0.0dev,>=2.4.0
 google-api-core<3.0.0,>=2.11
 grpcio-testing
 ipython
 kfp<3.0.0,>=2.6.0
@@ -134,22 +134,22 @@
 tensorflow<=2.12.0,>=2.3.0
 torch<2.1.0,>=2.0.0
 xgboost
 xgboost_ray
 requests-toolbelt<1.0.0
 
 [testing:python_version < "3.11"]
-ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 pyarrow<8.0dev,>=3.0.0
+ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 
 [testing:python_version >= "3.10"]
 bigframes
 
 [testing:python_version >= "3.11"]
-ray[default]<=2.9.3,>=2.5
 pyarrow>=10.0.1
+ray[default]<=2.9.3,>=2.5
 
 [vizier]
 google-vizier>=0.1.6
 
 [xai]
 tensorflow<3.0.0dev,>=2.3.0
```

