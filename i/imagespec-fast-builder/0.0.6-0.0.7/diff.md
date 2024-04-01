# Comparing `tmp/imagespec_fast_builder-0.0.6.tar.gz` & `tmp/imagespec_fast_builder-0.0.7.tar.gz`

## Comparing `imagespec_fast_builder-0.0.6.tar` & `imagespec_fast_builder-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/.github/workflows/wheel.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/dockerfiles/Dockerfile
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/dockerfiles/Dockerfile.base
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/experiments/build_wf.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/experiments/check_builder.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/src/imagespec_fast_builder/__init__.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/src/imagespec_fast_builder/_image_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/LICENSE
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/README.md
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/.github/workflows/wheel.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/dockerfiles/Dockerfile
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/dockerfiles/Dockerfile.base
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/experiments/build_wf.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/experiments/check_builder.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/src/imagespec_fast_builder/__init__.py
+-rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/src/imagespec_fast_builder/_image_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/README.md
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.7/PKG-INFO
```

### Comparing `imagespec_fast_builder-0.0.6/.github/workflows/wheel.yaml` & `imagespec_fast_builder-0.0.7/.github/workflows/wheel.yaml`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.6/dockerfiles/Dockerfile` & `imagespec_fast_builder-0.0.7/dockerfiles/Dockerfile`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.6/experiments/check_builder.py` & `imagespec_fast_builder-0.0.7/experiments/check_builder.py`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.6/src/imagespec_fast_builder/_image_builder.py` & `imagespec_fast_builder-0.0.7/src/imagespec_fast_builder/_image_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     --mount=type=bind,target=requirements.txt,src=requirements.txt \
     /root/.cargo/bin/uv \
     pip install --python /opt/conda/envs/dev/bin/python $PIP_INDEX \
     --verbose \
     --requirement requirements.txt
 """
 
-APT_INSTALL_COMMAND_TEMPLATE = Template("""\
+APT_INSTALL_COMMAND_TEMPLATE = Template(
+    """\
 RUN --mount=type=cache,target=/var/cache/apt,id=apt \
     apt-get update && apt-get install -y --no-install-recommends \
     $APT_PACKAGES
-""")
+"""
+)
 
 DOCKER_FILE_TEMPLATE = Template(
     """\
 #syntax=docker/dockerfile:1.5
 FROM thomasjpfan/fast-builder-base:0.0.1 as build
 
 RUN --mount=type=cache,target=/opt/conda/pkgs,id=conda \
@@ -58,25 +60,26 @@
 
 COPY --from=build /venv /venv
 ENV PATH="/venv/bin:$$PATH"
 
 WORKDIR /root
 ENV PYTHONPATH=/root FLYTE_SDK_RICH_TRACEBACKS=0 SSL_CERT_DIR=/etc/ssl/certs $ENV
 
+$RUN_COMMANDS
+
 RUN useradd --create-home --shell /bin/bash -u 1000 flytekit \
     && chown flytekit: /root \
     && chown flytekit: /home
 
 RUN echo "source /venv/bin/activate" >> /home/flytekit/.bashrc
 SHELL ["/bin/bash", "-c"]
 
 USER flytekit
 
 $COPY_COMMAND
-$RUN_COMMANDS
 """
 )
 
 
 def write_dockerfile(image_spec: ImageSpec, tmp_dir: Path):
     base_image = image_spec.base_image or "debian:bookworm-slim"
     pip_index = f"--index-url {image_spec.pip_index}" if image_spec.pip_index else ""
```

### Comparing `imagespec_fast_builder-0.0.6/.gitignore` & `imagespec_fast_builder-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.6/LICENSE` & `imagespec_fast_builder-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.6/README.md` & `imagespec_fast_builder-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.6/pyproject.toml` & `imagespec_fast_builder-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.6/PKG-INFO` & `imagespec_fast_builder-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: imagespec-fast-builder
-Version: 0.0.6
+Version: 0.0.7
 Summary: A faster ImageSpec builder for flytekit
 Project-URL: Issues, https://github.com/thomasjpfan/imagespec-fast-builder/issues
 Project-URL: Source, https://github.com/thomasjpfan/imagespec-fast-builder
 Author-email: "Thomas J. Fan" <thomasjpfan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

