# Comparing `tmp/kdp-python-connector-0.57.0.tar.gz` & `tmp/kdp-python-connector-0.58.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-python-connector-0.57.0.tar", last modified: Fri Mar 29 08:12:38 2024, max compression
+gzip compressed data, was "kdp-python-connector-0.58.0.tar", last modified: Mon Apr  1 15:54:35 2024, max compression
```

## Comparing `kdp-python-connector-0.57.0.tar` & `kdp-python-connector-0.58.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.260696 kdp-python-connector-0.57.0/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.248696 kdp-python-connector-0.57.0/.github/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.github/pull_request_template.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.248696 kdp-python-connector-0.57.0/.github/workflows/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6788 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.github/workflows/build-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6340 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.github/workflows/build-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.github/workflows/release-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.github/workflows/release-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.github/workflows/release.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.gitignore
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-03-29 08:12:38.260696 kdp-python-connector-0.57.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.248696 kdp-python-connector-0.57.0/datafiles/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/datafiles/actorfilms.csv
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.252696 kdp-python-connector-0.57.0/docs/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/Makefile
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/conf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/index.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/kdp_connector.configuration.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/kdp_connector.connectors.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/kdp_connector.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/make.bat
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/docs/modules.rst
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.252696 kdp-python-connector-0.57.0/kdp_connector/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.252696 kdp-python-connector-0.57.0/kdp_connector/configuration/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/configuration/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3068 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/configuration/authenticationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/configuration/configurationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/configuration/keycloak_authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      548 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/configuration/proxy_authentication.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.256696 kdp-python-connector-0.57.0/kdp_connector/connectors/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      668 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/Storage.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1584 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/audit_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3618 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/audit_log_configs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7467 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/batch_write.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2205 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/index_management.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/ingest_job_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8752 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/kdp_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2301 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/read.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/connectors/upload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25200 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/kdp_connector/main.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.256696 kdp-python-connector-0.57.0/kdp_python_connector.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-03-29 08:12:38.000000 kdp-python-connector-0.57.0/kdp_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-03-29 08:12:38.000000 kdp-python-connector-0.57.0/kdp_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-29 08:12:38.000000 kdp-python-connector-0.57.0/kdp_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-03-29 08:12:38.000000 kdp-python-connector-0.57.0/kdp_python_connector.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-03-29 08:12:38.000000 kdp-python-connector-0.57.0/kdp_python_connector.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-29 08:12:38.260696 kdp-python-connector-0.57.0/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 08:12:38.256696 kdp-python-connector-0.57.0/test/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/test/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4014 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/test/test_ingest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/test/test_keycloak.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4925 2024-03-29 08:12:27.000000 kdp-python-connector-0.57.0/test/test_read.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.876899 kdp-python-connector-0.58.0/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.848899 kdp-python-connector-0.58.0/.github/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/pull_request_template.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.848899 kdp-python-connector-0.58.0/.github/workflows/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6788 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/build-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6340 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/build-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/release-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/release-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/release.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.gitignore
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 15:54:35.876899 kdp-python-connector-0.58.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.852899 kdp-python-connector-0.58.0/datafiles/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/datafiles/actorfilms.csv
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.856899 kdp-python-connector-0.58.0/docs/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/Makefile
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/conf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/index.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/kdp_connector.configuration.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/kdp_connector.connectors.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/kdp_connector.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/make.bat
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/modules.rst
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.860899 kdp-python-connector-0.58.0/kdp_connector/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.860899 kdp-python-connector-0.58.0/kdp_connector/configuration/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/authenticationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/configurationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/keycloak_authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      549 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/proxy_authentication.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.868899 kdp-python-connector-0.58.0/kdp_connector/connectors/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/Storage.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3620 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log_configs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7467 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/batch_write.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2205 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/index_management.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/ingest_job_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8752 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/kdp_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2302 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/read.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/upload.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25203 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/main.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.872899 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-01 15:54:35.876899 kdp-python-connector-0.58.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.872899 kdp-python-connector-0.58.0/test/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4014 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/test_ingest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/test_keycloak.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/test_read.py
```

### Comparing `kdp-python-connector-0.57.0/.github/workflows/build-internal.yaml` & `kdp-python-connector-0.58.0/.github/workflows/build-internal.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/.github/workflows/build-public.yaml` & `kdp-python-connector-0.58.0/.github/workflows/build-public.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/.github/workflows/release-internal.yaml` & `kdp-python-connector-0.58.0/.github/workflows/release-internal.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/.github/workflows/release-public.yaml` & `kdp-python-connector-0.58.0/.github/workflows/release-public.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/.github/workflows/release.yaml` & `kdp-python-connector-0.58.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/.gitignore` & `kdp-python-connector-0.58.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/PKG-INFO` & `kdp-python-connector-0.58.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.57.0
+Version: 0.58.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `kdp-python-connector-0.57.0/datafiles/actorfilms.csv` & `kdp-python-connector-0.58.0/datafiles/actorfilms.csv`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/docs/Makefile` & `kdp-python-connector-0.58.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/docs/conf.py` & `kdp-python-connector-0.58.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/docs/kdp_connector.configuration.rst` & `kdp-python-connector-0.58.0/docs/kdp_connector.configuration.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/docs/kdp_connector.connectors.rst` & `kdp-python-connector-0.58.0/docs/kdp_connector.connectors.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/docs/make.bat` & `kdp-python-connector-0.58.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/configuration/authenticationUtil.py` & `kdp-python-connector-0.58.0/kdp_connector/configuration/authenticationUtil.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import kdp_api
 
 from kdp_api.api.authenticate_api import Authentication
 from kdp_api.api.authenticate_api import AuthenticateApi
-from kdp_api.model.authentication_sso import AuthenticationSSO
+from kdp_api.models.authentication_sso import AuthenticationSSO
 from kdp_connector.configuration.keycloak_authentication import KeycloakAuthentication
 from kdp_connector.configuration.proxy_authentication import ProxyAuthentication
 
 
 class AuthenticationUtil(object):
 
     @staticmethod
```

### Comparing `kdp-python-connector-0.57.0/kdp_connector/configuration/configurationUtil.py` & `kdp-python-connector-0.58.0/kdp_connector/configuration/configurationUtil.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/configuration/keycloak_authentication.py` & `kdp-python-connector-0.58.0/kdp_connector/configuration/keycloak_authentication.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/configuration/proxy_authentication.py` & `kdp-python-connector-0.58.0/kdp_connector/configuration/proxy_authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kdp_api.model.authentication import Authentication
+from kdp_api.models.authentication import Authentication
 
 """
 This class extends Authentication and override the allowed_values field to allow
 authentication request coming from auth-proxy service.
 """
 class ProxyAuthentication(Authentication):
     allowed_values = {
```

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/Storage.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/Storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import kdp_api
 from kdp_api.api import manage_records_api
-from kdp_api.model.job import Job
+from kdp_api.models.job import Job
 
 class StorageApi(object):
 
     def clear_dataset(self, config, dataset_id: str) -> Job:
         """This method will be used to clear dataset.
 
             :param Configuration config: Connection configuration
```

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/audit_log.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import kdp_api
 import logging
 from kdp_api.api import workspaces_api
-from kdp_api.model.audit_log_paginator import AuditLogPaginator
+from kdp_api.models.audit_log_paginator import AuditLogPaginator
 from kdp_api.configuration import Configuration
 
 
 class AuditLogApi(object):
     def __init__(self, configuration: Configuration=None):
         self.configuration = configuration
```

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/audit_log_configs.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import kdp_api
 import logging
 from kdp_api.api import workspaces_api
-from kdp_api.model.audit_log_configuration_paginator import AuditLogConfigurationPaginator
-from kdp_api.model.audit_log_configuration import AuditLogConfiguration
+from kdp_api.models.audit_log_configuration_paginator import AuditLogConfigurationPaginator
+from kdp_api.models.audit_log_configuration import AuditLogConfiguration
 from kdp_api.configuration import Configuration
 
 
 class AuditLogConfigsApi(object):
     def __init__(self, configuration: Configuration=None):
         self.configuration = configuration
```

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/batch_write.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/batch_write.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/index_management.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/index_management.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/ingest_job_api.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/ingest_job_api.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/kdp_api.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/kdp_api.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/query.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import kdp_api
 from kdp_api.api import read_and_query_api
-from kdp_api.model.query_document_lucene_response import QueryDocumentLuceneResponse
+from kdp_api.models.query_document_lucene_response import QueryDocumentLuceneResponse
 
 class QueryApi(object):
 
     def post_lucene_query(self, config, dataset_id: str, expression: str, limit: int = 5, offset: int = 0):
         """This method will be used to query data in KDP datasets using the lucene syntax
 
             :param Configuration config: Connection configuration
```

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/read.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/read.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/connectors/upload.py` & `kdp-python-connector-0.58.0/kdp_connector/connectors/upload.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/kdp_connector/main.py` & `kdp-python-connector-0.58.0/kdp_connector/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from kdp_connector.connectors.query import QueryApi
 from kdp_connector.connectors.index_management import IndexManagementApi
 from kdp_connector.connectors.upload import UploadApi
 from kdp_connector.connectors.Storage import StorageApi
 from kdp_connector.connectors.audit_log import AuditLogApi
 from kdp_connector.connectors.audit_log_configs import AuditLogConfigsApi
 from kdp_api.models import SecurityLabelInfoParams
-from kdp_api.model.audit_log_configuration_paginator import AuditLogConfigurationPaginator
-from kdp_api.model.audit_log_configuration import AuditLogConfiguration
-from kdp_api.model.audit_log_paginator import AuditLogPaginator
+from kdp_api.models.audit_log_configuration_paginator import AuditLogConfigurationPaginator
+from kdp_api.models.audit_log_configuration import AuditLogConfiguration
+from kdp_api.models.audit_log_paginator import AuditLogPaginator
 from pandas import DataFrame
 
 class KdpConn(object):
     """This class contains convenience methods used for interacting with KDP"""
 
     def __init__(self, path_to_ca_file: str = '', host: str = 'https://api.app.koverse.com',
                  discard_unknown_keys: bool = True):
```

### Comparing `kdp-python-connector-0.57.0/kdp_python_connector.egg-info/PKG-INFO` & `kdp-python-connector-0.58.0/kdp_python_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.57.0
+Version: 0.58.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `kdp-python-connector-0.57.0/kdp_python_connector.egg-info/SOURCES.txt` & `kdp-python-connector-0.58.0/kdp_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/pyproject.toml` & `kdp-python-connector-0.58.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "0.57.0"
+version = "0.58.0"
 dependencies = [
   'kdp-api-python-client ~= 4.124.0',
   'pandas ~= 1.4.2',
   'numpy ~= 1.22.4'
 ]
 
 [tool.setuptools.packages.find]
```

### Comparing `kdp-python-connector-0.57.0/test/test_ingest.py` & `kdp-python-connector-0.58.0/test/test_ingest.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/test/test_keycloak.py` & `kdp-python-connector-0.58.0/test/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.57.0/test/test_read.py` & `kdp-python-connector-0.58.0/test/test_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from unittest.mock import Mock, call, ANY
 
-from kdp_api.model.json_record import JsonRecord
+from kdp_api.models.json_record import JsonRecord
 from pandas._testing import assert_frame_equal
 
 import pandas as pd
 
 from kdp_connector.connectors.read import ReadApi
 from kdp_api.models import RecordBatch
 from kdp_connector.main import KdpConn
```

