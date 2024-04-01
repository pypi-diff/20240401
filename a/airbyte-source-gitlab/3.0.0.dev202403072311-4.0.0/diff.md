# Comparing `tmp/airbyte_source_gitlab-3.0.0.dev202403072311.tar.gz` & `tmp/airbyte_source_gitlab-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_gitlab-3.0.0.dev202403072311.tar", max compression
+gzip compressed data, was "airbyte_source_gitlab-4.0.0.tar", max compression
```

## Comparing `airbyte_source_gitlab-3.0.0.dev202403072311.tar` & `airbyte_source_gitlab-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     4496 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/README.md
--rw-r--r--   0        0        0      780 2024-03-07 23:11:53.816452 airbyte_source_gitlab-3.0.0.dev202403072311/pyproject.toml
--rw-r--r--   0        0        0     1134 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/__init__.py
--rw-r--r--   0        0        0     3816 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/config_migrations.py
--rw-r--r--   0        0        0      403 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/run.py
--rw-r--r--   0        0        0      800 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/branches.json
--rw-r--r--   0        0        0     1676 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/commits.json
--rw-r--r--   0        0        0     5084 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/deployments.json
--rw-r--r--   0        0        0     5472 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/epic_issues.json
--rw-r--r--   0        0        0     2790 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/epics.json
--rw-r--r--   0        0        0     1687 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_issue_boards.json
--rw-r--r--   0        0        0      785 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_labels.json
--rw-r--r--   0        0        0     1261 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_members.json
--rw-r--r--   0        0        0      898 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_milestones.json
--rw-r--r--   0        0        0     4148 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/groups.json
--rw-r--r--   0        0        0     6304 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/issues.json
--rw-r--r--   0        0        0     2275 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/jobs.json
--rw-r--r--   0        0        0     1744 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/merge_request_commits.json
--rw-r--r--   0        0        0     4388 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/merge_requests.json
--rw-r--r--   0        0        0      777 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/pipelines.json
--rw-r--r--   0        0        0     2041 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/pipelines_extended.json
--rw-r--r--   0        0        0      913 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/project_labels.json
--rw-r--r--   0        0        0     1263 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/project_members.json
--rw-r--r--   0        0        0      900 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/project_milestones.json
--rw-r--r--   0        0        0    12131 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/projects.json
--rw-r--r--   0        0        0     1781 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/releases.json
--rw-r--r--   0        0        0      771 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/tags.json
--rw-r--r--   0        0        0      496 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/users.json
--rw-r--r--   0        0        0    12072 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/source.py
--rw-r--r--   0        0        0     6132 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/spec.json
--rw-r--r--   0        0        0    16122 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/streams.py
--rw-r--r--   0        0        0      456 2024-03-07 23:08:40.684353 airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/utils.py
--rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 airbyte_source_gitlab-3.0.0.dev202403072311/PKG-INFO
+-rw-r--r--   0        0        0     4501 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/README.md
+-rw-r--r--   0        0        0      758 2024-04-01 16:57:17.527042 airbyte_source_gitlab-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1134 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/__init__.py
+-rw-r--r--   0        0        0     2054 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/components/partition_routers.py
+-rw-r--r--   0        0        0     3816 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/config_migrations.py
+-rw-r--r--   0        0        0    20701 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/manifest.yaml
+-rw-r--r--   0        0        0      403 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/run.py
+-rw-r--r--   0        0        0      800 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/branches.json
+-rw-r--r--   0        0        0     1676 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/commits.json
+-rw-r--r--   0        0        0     5084 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/deployments.json
+-rw-r--r--   0        0        0     5472 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/epic_issues.json
+-rw-r--r--   0        0        0     2790 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/epics.json
+-rw-r--r--   0        0        0     1687 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_issue_boards.json
+-rw-r--r--   0        0        0      785 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_labels.json
+-rw-r--r--   0        0        0     1261 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_members.json
+-rw-r--r--   0        0        0      898 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_milestones.json
+-rw-r--r--   0        0        0     4148 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/groups.json
+-rw-r--r--   0        0        0     6304 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/issues.json
+-rw-r--r--   0        0        0     2275 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/jobs.json
+-rw-r--r--   0        0        0     1744 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/merge_request_commits.json
+-rw-r--r--   0        0        0     4388 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/merge_requests.json
+-rw-r--r--   0        0        0      777 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/pipelines.json
+-rw-r--r--   0        0        0     2041 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/pipelines_extended.json
+-rw-r--r--   0        0        0      913 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/project_labels.json
+-rw-r--r--   0        0        0     1263 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/project_members.json
+-rw-r--r--   0        0        0      900 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/project_milestones.json
+-rw-r--r--   0        0        0    12131 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/projects.json
+-rw-r--r--   0        0        0     1781 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/releases.json
+-rw-r--r--   0        0        0      771 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/tags.json
+-rw-r--r--   0        0        0      496 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/schemas/users.json
+-rw-r--r--   0        0        0     1093 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/source.py
+-rw-r--r--   0        0        0     6132 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/spec.json
+-rw-r--r--   0        0        0      456 2024-04-01 14:47:10.000000 airbyte_source_gitlab-4.0.0/source_gitlab/utils.py
+-rw-r--r--   0        0        0     5234 1970-01-01 00:00:00.000000 airbyte_source_gitlab-4.0.0/PKG-INFO
```

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/README.md` & `airbyte_source_gitlab-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-gitlab spec
 poetry run source-gitlab check --config secrets/config.json
 poetry run source-gitlab discover --config secrets/config.json
-poetry run source-gitlab read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-gitlab read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/pyproject.toml` & `airbyte_source_gitlab-4.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.0.dev202403072311"
+version = "4.0.0"
 name = "airbyte-source-gitlab"
 description = "Source implementation for GitLab."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_gitlab" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "==0.58.8"
+airbyte-cdk = "^0"
 vcrpy = "==4.1.1"
 
 [tool.poetry.scripts]
 source-gitlab = "source_gitlab.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.12.0"
```

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/__init__.py` & `airbyte_source_gitlab-4.0.0/source_gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/config_migrations.py` & `airbyte_source_gitlab-4.0.0/source_gitlab/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/branches.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/branches.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/commits.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/deployments.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/deployments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/epic_issues.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/epic_issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/epics.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/epics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_issue_boards.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_issue_boards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_labels.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_members.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/group_milestones.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/group_milestones.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/groups.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/issues.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/jobs.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/merge_request_commits.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/merge_request_commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/merge_requests.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/merge_requests.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/pipelines.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/pipelines_extended.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/pipelines_extended.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/project_labels.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/project_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/project_members.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/project_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/project_milestones.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/project_milestones.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/projects.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/releases.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/releases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/schemas/tags.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/schemas/tags.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/source_gitlab/spec.json` & `airbyte_source_gitlab-4.0.0/source_gitlab/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-3.0.0.dev202403072311/PKG-INFO` & `airbyte_source_gitlab-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-gitlab
-Version: 3.0.0.dev202403072311
+Version: 4.0.0
 Summary: Source implementation for GitLab.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.58.8)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Requires-Dist: vcrpy (==4.1.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/gitlab
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Gitlab source connector
 
@@ -46,15 +46,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-gitlab spec
 poetry run source-gitlab check --config secrets/config.json
 poetry run source-gitlab discover --config secrets/config.json
-poetry run source-gitlab read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-gitlab read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

