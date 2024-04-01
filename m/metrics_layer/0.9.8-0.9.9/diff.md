# Comparing `tmp/metrics_layer-0.9.8.tar.gz` & `tmp/metrics_layer-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrics_layer-0.9.8.tar", max compression
+gzip compressed data, was "metrics_layer-0.9.9.tar", max compression
```

## Comparing `metrics_layer-0.9.8.tar` & `metrics_layer-0.9.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11357 2022-04-12 04:32:23.996095 metrics_layer-0.9.8/LICENSE
--rw-r--r--   0        0        0     2999 2022-09-23 22:25:22.029268 metrics_layer-0.9.8/README.md
--rw-r--r--   0        0        0      278 2022-09-26 21:24:52.626336 metrics_layer-0.9.8/metrics_layer/__init__.py
--rw-r--r--   0        0        0       36 2022-04-12 04:32:23.996479 metrics_layer-0.9.8/metrics_layer/cli/__init__.py
--rw-r--r--   0        0        0     7533 2022-10-03 14:43:08.968783 metrics_layer-0.9.8/metrics_layer/cli/cli_commands.py
--rw-r--r--   0        0        0    18094 2022-10-04 17:40:01.241050 metrics_layer-0.9.8/metrics_layer/cli/seeding.py
--rw-r--r--   0        0        0      141 2022-04-12 04:32:23.996919 metrics_layer-0.9.8/metrics_layer/core/__init__.py
--rw-r--r--   0        0        0       42 2022-04-12 04:32:23.997041 metrics_layer-0.9.8/metrics_layer/core/convert/__init__.py
--rw-r--r--   0        0        0     8519 2022-09-20 01:33:29.132753 metrics_layer-0.9.8/metrics_layer/core/convert/convert.py
--rw-r--r--   0        0        0      481 2022-08-26 15:49:36.926285 metrics_layer-0.9.8/metrics_layer/core/exceptions.py
--rw-r--r--   0        0        0       82 2022-04-12 04:32:23.997268 metrics_layer-0.9.8/metrics_layer/core/model/__init__.py
--rw-r--r--   0        0        0     1386 2022-07-21 23:52:32.402601 metrics_layer-0.9.8/metrics_layer/core/model/base.py
--rw-r--r--   0        0        0     5828 2022-09-14 22:17:29.053028 metrics_layer-0.9.8/metrics_layer/core/model/dashboard.py
--rw-r--r--   0        0        0      168 2022-09-19 21:01:54.294759 metrics_layer-0.9.8/metrics_layer/core/model/definitions.py
--rw-r--r--   0        0        0     4717 2022-07-21 23:52:32.403069 metrics_layer-0.9.8/metrics_layer/core/model/explore.py
--rw-r--r--   0        0        0    35520 2022-10-02 13:49:02.843817 metrics_layer-0.9.8/metrics_layer/core/model/field.py
--rw-r--r--   0        0        0    21076 2022-09-20 01:33:29.133975 metrics_layer-0.9.8/metrics_layer/core/model/filter.py
--rw-r--r--   0        0        0     7053 2022-07-21 23:52:32.403996 metrics_layer-0.9.8/metrics_layer/core/model/join.py
--rw-r--r--   0        0        0    15014 2022-09-20 01:33:29.134626 metrics_layer-0.9.8/metrics_layer/core/model/join_graph.py
--rw-r--r--   0        0        0     2793 2022-09-20 01:33:29.135104 metrics_layer-0.9.8/metrics_layer/core/model/model.py
--rw-r--r--   0        0        0    14560 2022-10-04 21:15:55.277724 metrics_layer-0.9.8/metrics_layer/core/model/project.py
--rw-r--r--   0        0        0     3081 2022-07-21 23:52:32.404739 metrics_layer-0.9.8/metrics_layer/core/model/set.py
--rw-r--r--   0        0        0     7614 2022-10-04 21:16:07.820722 metrics_layer-0.9.8/metrics_layer/core/model/view.py
--rw-r--r--   0        0        0      240 2022-09-19 21:01:54.295038 metrics_layer-0.9.8/metrics_layer/core/parse/__init__.py
--rw-r--r--   0        0        0     5493 2022-09-19 21:01:54.295221 metrics_layer-0.9.8/metrics_layer/core/parse/connections.py
--rw-r--r--   0        0        0     3667 2022-10-04 19:12:50.509346 metrics_layer-0.9.8/metrics_layer/core/parse/github_repo.py
--rw-r--r--   0        0        0     2226 2022-10-04 21:16:51.827657 metrics_layer-0.9.8/metrics_layer/core/parse/manifest.py
--rw-r--r--   0        0        0     3890 2022-09-27 16:27:02.161075 metrics_layer-0.9.8/metrics_layer/core/parse/project_dumper.py
--rw-r--r--   0        0        0     5435 2022-10-04 17:42:30.100234 metrics_layer-0.9.8/metrics_layer/core/parse/project_loader.py
--rw-r--r--   0        0        0     3835 2022-10-04 19:12:54.465736 metrics_layer-0.9.8/metrics_layer/core/parse/project_reader_base.py
--rw-r--r--   0        0        0     7486 2022-10-04 23:54:30.715391 metrics_layer-0.9.8/metrics_layer/core/parse/project_reader_dbt.py
--rw-r--r--   0        0        0     2305 2022-10-04 19:12:00.793108 metrics_layer-0.9.8/metrics_layer/core/parse/project_reader_metrics_layer.py
--rw-r--r--   0        0        0       50 2022-04-12 04:32:23.999685 metrics_layer-0.9.8/metrics_layer/core/query/__init__.py
--rw-r--r--   0        0        0    10650 2022-10-04 22:16:03.219541 metrics_layer-0.9.8/metrics_layer/core/query/query.py
--rw-r--r--   0        0        0       92 2022-04-12 04:32:23.999904 metrics_layer-0.9.8/metrics_layer/core/sql/__init__.py
--rw-r--r--   0        0        0    13049 2022-09-23 23:17:56.694483 metrics_layer-0.9.8/metrics_layer/core/sql/merged_query_resolve.py
--rw-r--r--   0        0        0     2531 2022-08-26 15:49:36.928259 metrics_layer-0.9.8/metrics_layer/core/sql/query_base.py
--rw-r--r--   0        0        0    17237 2022-09-14 22:16:46.718652 metrics_layer-0.9.8/metrics_layer/core/sql/query_cumulative_metric.py
--rw-r--r--   0        0        0    11637 2022-09-14 22:17:59.294757 metrics_layer-0.9.8/metrics_layer/core/sql/query_design.py
--rw-r--r--   0        0        0     1288 2022-04-12 04:32:24.000178 metrics_layer-0.9.8/metrics_layer/core/sql/query_dialect.py
--rw-r--r--   0        0        0       81 2022-04-12 04:32:24.000241 metrics_layer-0.9.8/metrics_layer/core/sql/query_errors.py
--rw-r--r--   0        0        0     8724 2022-09-14 22:18:11.463203 metrics_layer-0.9.8/metrics_layer/core/sql/query_filter.py
--rw-r--r--   0        0        0    11532 2022-09-14 22:18:27.413707 metrics_layer-0.9.8/metrics_layer/core/sql/query_funnel.py
--rw-r--r--   0        0        0    12160 2022-10-04 19:12:58.783166 metrics_layer-0.9.8/metrics_layer/core/sql/query_generator.py
--rw-r--r--   0        0        0     3660 2022-08-26 15:49:36.929341 metrics_layer-0.9.8/metrics_layer/core/sql/query_merged_results.py
--rw-r--r--   0        0        0     5931 2022-08-02 18:59:43.581905 metrics_layer-0.9.8/metrics_layer/core/sql/query_runner.py
--rw-r--r--   0        0        0     4436 2022-09-20 01:33:29.136919 metrics_layer-0.9.8/metrics_layer/core/sql/resolve.py
--rw-r--r--   0        0        0     7678 2022-09-20 01:33:29.137408 metrics_layer-0.9.8/metrics_layer/core/sql/single_query_resolve.py
--rw-r--r--   0        0        0      399 2022-09-19 21:01:54.298359 metrics_layer-0.9.8/metrics_layer/core/utils.py
--rw-r--r--   0        0        0     2053 2022-10-04 23:55:43.256384 metrics_layer-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 metrics_layer-0.9.8/setup.py
--rw-r--r--   0        0        0     4914 1970-01-01 00:00:00.000000 metrics_layer-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-04-12 04:32:23.996095 metrics_layer-0.9.9/LICENSE
+-rw-r--r--   0        0        0     2999 2022-09-23 22:25:22.029268 metrics_layer-0.9.9/README.md
+-rw-r--r--   0        0        0      278 2022-09-26 21:24:52.626336 metrics_layer-0.9.9/metrics_layer/__init__.py
+-rw-r--r--   0        0        0       36 2022-04-12 04:32:23.996479 metrics_layer-0.9.9/metrics_layer/cli/__init__.py
+-rw-r--r--   0        0        0     7533 2022-10-03 14:43:08.968783 metrics_layer-0.9.9/metrics_layer/cli/cli_commands.py
+-rw-r--r--   0        0        0    18094 2022-10-04 17:40:01.241050 metrics_layer-0.9.9/metrics_layer/cli/seeding.py
+-rw-r--r--   0        0        0      141 2022-04-12 04:32:23.996919 metrics_layer-0.9.9/metrics_layer/core/__init__.py
+-rw-r--r--   0        0        0       42 2022-04-12 04:32:23.997041 metrics_layer-0.9.9/metrics_layer/core/convert/__init__.py
+-rw-r--r--   0        0        0     8519 2022-09-20 01:33:29.132753 metrics_layer-0.9.9/metrics_layer/core/convert/convert.py
+-rw-r--r--   0        0        0      481 2022-08-26 15:49:36.926285 metrics_layer-0.9.9/metrics_layer/core/exceptions.py
+-rw-r--r--   0        0        0       82 2022-04-12 04:32:23.997268 metrics_layer-0.9.9/metrics_layer/core/model/__init__.py
+-rw-r--r--   0        0        0     1386 2022-07-21 23:52:32.402601 metrics_layer-0.9.9/metrics_layer/core/model/base.py
+-rw-r--r--   0        0        0     5828 2022-09-14 22:17:29.053028 metrics_layer-0.9.9/metrics_layer/core/model/dashboard.py
+-rw-r--r--   0        0        0      168 2022-09-19 21:01:54.294759 metrics_layer-0.9.9/metrics_layer/core/model/definitions.py
+-rw-r--r--   0        0        0     4717 2022-07-21 23:52:32.403069 metrics_layer-0.9.9/metrics_layer/core/model/explore.py
+-rw-r--r--   0        0        0    35520 2022-10-02 13:49:02.843817 metrics_layer-0.9.9/metrics_layer/core/model/field.py
+-rw-r--r--   0        0        0    21076 2022-09-20 01:33:29.133975 metrics_layer-0.9.9/metrics_layer/core/model/filter.py
+-rw-r--r--   0        0        0     7053 2022-07-21 23:52:32.403996 metrics_layer-0.9.9/metrics_layer/core/model/join.py
+-rw-r--r--   0        0        0    15014 2022-09-20 01:33:29.134626 metrics_layer-0.9.9/metrics_layer/core/model/join_graph.py
+-rw-r--r--   0        0        0     2793 2022-09-20 01:33:29.135104 metrics_layer-0.9.9/metrics_layer/core/model/model.py
+-rw-r--r--   0        0        0    14560 2022-10-04 21:15:55.277724 metrics_layer-0.9.9/metrics_layer/core/model/project.py
+-rw-r--r--   0        0        0     3081 2022-07-21 23:52:32.404739 metrics_layer-0.9.9/metrics_layer/core/model/set.py
+-rw-r--r--   0        0        0     7614 2022-10-04 21:16:07.820722 metrics_layer-0.9.9/metrics_layer/core/model/view.py
+-rw-r--r--   0        0        0      240 2022-09-19 21:01:54.295038 metrics_layer-0.9.9/metrics_layer/core/parse/__init__.py
+-rw-r--r--   0        0        0     5493 2022-09-19 21:01:54.295221 metrics_layer-0.9.9/metrics_layer/core/parse/connections.py
+-rw-r--r--   0        0        0     3667 2022-10-04 19:12:50.509346 metrics_layer-0.9.9/metrics_layer/core/parse/github_repo.py
+-rw-r--r--   0        0        0     2226 2022-10-04 21:16:51.827657 metrics_layer-0.9.9/metrics_layer/core/parse/manifest.py
+-rw-r--r--   0        0        0     3890 2022-09-27 16:27:02.161075 metrics_layer-0.9.9/metrics_layer/core/parse/project_dumper.py
+-rw-r--r--   0        0        0     5435 2022-10-04 17:42:30.100234 metrics_layer-0.9.9/metrics_layer/core/parse/project_loader.py
+-rw-r--r--   0        0        0     3967 2022-10-05 14:14:43.462365 metrics_layer-0.9.9/metrics_layer/core/parse/project_reader_base.py
+-rw-r--r--   0        0        0     7542 2022-10-05 14:15:37.670162 metrics_layer-0.9.9/metrics_layer/core/parse/project_reader_dbt.py
+-rw-r--r--   0        0        0     2305 2022-10-04 19:12:00.793108 metrics_layer-0.9.9/metrics_layer/core/parse/project_reader_metrics_layer.py
+-rw-r--r--   0        0        0       50 2022-04-12 04:32:23.999685 metrics_layer-0.9.9/metrics_layer/core/query/__init__.py
+-rw-r--r--   0        0        0    10650 2022-10-04 22:16:03.219541 metrics_layer-0.9.9/metrics_layer/core/query/query.py
+-rw-r--r--   0        0        0       92 2022-04-12 04:32:23.999904 metrics_layer-0.9.9/metrics_layer/core/sql/__init__.py
+-rw-r--r--   0        0        0    13049 2022-09-23 23:17:56.694483 metrics_layer-0.9.9/metrics_layer/core/sql/merged_query_resolve.py
+-rw-r--r--   0        0        0     2531 2022-08-26 15:49:36.928259 metrics_layer-0.9.9/metrics_layer/core/sql/query_base.py
+-rw-r--r--   0        0        0    17237 2022-09-14 22:16:46.718652 metrics_layer-0.9.9/metrics_layer/core/sql/query_cumulative_metric.py
+-rw-r--r--   0        0        0    11637 2022-09-14 22:17:59.294757 metrics_layer-0.9.9/metrics_layer/core/sql/query_design.py
+-rw-r--r--   0        0        0     1288 2022-04-12 04:32:24.000178 metrics_layer-0.9.9/metrics_layer/core/sql/query_dialect.py
+-rw-r--r--   0        0        0       81 2022-04-12 04:32:24.000241 metrics_layer-0.9.9/metrics_layer/core/sql/query_errors.py
+-rw-r--r--   0        0        0     8724 2022-09-14 22:18:11.463203 metrics_layer-0.9.9/metrics_layer/core/sql/query_filter.py
+-rw-r--r--   0        0        0    11532 2022-09-14 22:18:27.413707 metrics_layer-0.9.9/metrics_layer/core/sql/query_funnel.py
+-rw-r--r--   0        0        0    12160 2022-10-04 19:12:58.783166 metrics_layer-0.9.9/metrics_layer/core/sql/query_generator.py
+-rw-r--r--   0        0        0     3660 2022-08-26 15:49:36.929341 metrics_layer-0.9.9/metrics_layer/core/sql/query_merged_results.py
+-rw-r--r--   0        0        0     5931 2022-08-02 18:59:43.581905 metrics_layer-0.9.9/metrics_layer/core/sql/query_runner.py
+-rw-r--r--   0        0        0     4436 2022-09-20 01:33:29.136919 metrics_layer-0.9.9/metrics_layer/core/sql/resolve.py
+-rw-r--r--   0        0        0     7678 2022-09-20 01:33:29.137408 metrics_layer-0.9.9/metrics_layer/core/sql/single_query_resolve.py
+-rw-r--r--   0        0        0      399 2022-09-19 21:01:54.298359 metrics_layer-0.9.9/metrics_layer/core/utils.py
+-rw-r--r--   0        0        0     2053 2022-10-05 14:17:53.831246 metrics_layer-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 metrics_layer-0.9.9/setup.py
+-rw-r--r--   0        0        0     4914 1970-01-01 00:00:00.000000 metrics_layer-0.9.9/PKG-INFO
```

### Comparing `metrics_layer-0.9.8/LICENSE` & `metrics_layer-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/README.md` & `metrics_layer-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/cli/cli_commands.py` & `metrics_layer-0.9.9/metrics_layer/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/cli/seeding.py` & `metrics_layer-0.9.9/metrics_layer/cli/seeding.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/convert/convert.py` & `metrics_layer-0.9.9/metrics_layer/core/convert/convert.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/base.py` & `metrics_layer-0.9.9/metrics_layer/core/model/base.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/dashboard.py` & `metrics_layer-0.9.9/metrics_layer/core/model/dashboard.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/explore.py` & `metrics_layer-0.9.9/metrics_layer/core/model/explore.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/field.py` & `metrics_layer-0.9.9/metrics_layer/core/model/field.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/filter.py` & `metrics_layer-0.9.9/metrics_layer/core/model/filter.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/join.py` & `metrics_layer-0.9.9/metrics_layer/core/model/join.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/join_graph.py` & `metrics_layer-0.9.9/metrics_layer/core/model/join_graph.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/model.py` & `metrics_layer-0.9.9/metrics_layer/core/model/model.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/project.py` & `metrics_layer-0.9.9/metrics_layer/core/model/project.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/set.py` & `metrics_layer-0.9.9/metrics_layer/core/model/set.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/model/view.py` & `metrics_layer-0.9.9/metrics_layer/core/model/view.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/connections.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/connections.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/github_repo.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/github_repo.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/manifest.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/manifest.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/project_dumper.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/project_dumper.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/project_loader.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/project_loader.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/project_reader_base.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/project_reader_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,22 @@
     def dashboards(self):
         if self.unloaded:
             self.load()
         return self._dashboards
 
     @property
     def zenlytic_project(self):
+        return self.read_yaml_if_exists(self.zenlytic_project_path)
+
+    @property
+    def zenlytic_project_path(self):
         zenlytic_project = self.read_yaml_if_exists(os.path.join(self.repo.folder, "zenlytic_project.yml"))
         if zenlytic_project:
-            return zenlytic_project
-        return self.read_yaml_if_exists(os.path.join(self.dbt_folder, "zenlytic_project.yml"))
+            return os.path.join(self.repo.folder, "zenlytic_project.yml")
+        return os.path.join(self.dbt_folder, "zenlytic_project.yml")
 
     @property
     def dbt_project(self):
         return self.read_yaml_if_exists(os.path.join(self.dbt_folder, "dbt_project.yml"))
 
     @property
     def dbt_folder(self):
```

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/project_reader_dbt.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/project_reader_dbt.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,17 @@
             self.profile_name = self.zenlytic_project.get("profile", dbt_profile_name)
         else:
             self.profile_name = dbt_profile_name
 
         models, views = self.parse_dbt_manifest(self.manifest)
         if self.zenlytic_project:
             paths = self.zenlytic_project.get("dashboard-paths", [])
-            dashboards = self._load_dbt_dashboards([os.path.join(self.repo.folder, dp) for dp in paths])
+            dashboards = self._load_dbt_dashboards(
+                [os.path.join(os.path.dirname(self.zenlytic_project_path), dp) for dp in paths]
+            )
         else:
             dashboards = []
 
         return models, views, dashboards
 
     def parse_dbt_manifest(self, manifest: dict):
         views = self._load_dbt_views(manifest)
@@ -41,15 +43,14 @@
             dashboards.extend(self._load_dashboards_from_folder(folder))
 
         return dashboards
 
     def _load_dashboards_from_folder(self, dashboard_folder: str):
         file_names = BaseRepo.glob_search(dashboard_folder, "*.yml")
         file_names += BaseRepo.glob_search(dashboard_folder, "*.yaml")
-
         dashboards = []
         for fn in file_names:
             yaml_dict = self.read_yaml_file(fn)
 
             # Handle keyerror
             if "type" not in yaml_dict:
                 print(f"WARNING: file {fn} is missing a type")
```

### Comparing `metrics_layer-0.9.8/metrics_layer/core/parse/project_reader_metrics_layer.py` & `metrics_layer-0.9.9/metrics_layer/core/parse/project_reader_metrics_layer.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/query/query.py` & `metrics_layer-0.9.9/metrics_layer/core/query/query.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/merged_query_resolve.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/merged_query_resolve.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_base.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_base.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_cumulative_metric.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_cumulative_metric.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_design.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_design.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_dialect.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_dialect.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_filter.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_filter.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_funnel.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_funnel.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_generator.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_generator.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_merged_results.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_merged_results.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/query_runner.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/query_runner.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/resolve.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/resolve.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/metrics_layer/core/sql/single_query_resolve.py` & `metrics_layer-0.9.9/metrics_layer/core/sql/single_query_resolve.py`

 * *Files identical despite different names*

### Comparing `metrics_layer-0.9.8/pyproject.toml` & `metrics_layer-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metrics_layer"
-version = "0.9.8"
+version = "0.9.9"
 description = "The open source metrics layer."
 authors = ["Paul Blankley <paul@zenlytic.com>"]
 keywords = ["Metrics Layer", "Looker", "Analytics"]
 readme = "README.md"
 license = "Apache 2.0"
 homepage = "https://github.com/Zenlytic/metrics_layer"
 repository = "https://github.com/Zenlytic/metrics_layer"
```

### Comparing `metrics_layer-0.9.8/setup.py` & `metrics_layer-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 entry_points = \
 {'console_scripts': ['metrics_layer = metrics_layer:cli_group',
                      'ml = metrics_layer:cli_group']}
 
 setup_kwargs = {
     'name': 'metrics-layer',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'The open source metrics layer.',
     'long_description': '# Metrics Layer\n\n[![Build Status](https://app.travis-ci.com/Zenlytic/metrics_layer.svg?branch=master)](https://app.travis-ci.com/Zenlytic/metrics_layer)\n[![codecov](https://codecov.io/gh/Zenlytic/metrics_layer/branch/master/graph/badge.svg?token=7JA6PKNV57)](https://codecov.io/gh/Zenlytic/metrics_layer)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# What is a Metrics Layer?\n\nMetrics Layer is an open source project with the goal of making access to metrics consistent throughout an organization. We believe you should be able to access consistent metrics from any tool you use to access data. This metrics layer is designed to work with [Zenlytic](https://zenlytic.com) as a BI tool. \n\n## How does it work?\n\nRight now, [Zenlytic](https://zenlytic.com) is the only supported BI tool. The Metrics Layer will read your data model and give you the ability to access those metrics and dimensions in a python client library, or through SQL with a special `MQL` tag.\n\nSound interesting? Here\'s how to set Metrics Layer up with your data model and start querying your metrics in **in under 2 minutes**.\n\n## Installation\n\nMake sure that your data warehouse is one of the supported types. Metrics Layer currently supports Snowflake, BigQuery and Redshift, and only works with `python >= 3.8`.\n\nInstall Metrics Layer with the appropriate extra for your warehouse\n\nFor Snowflake run `pip install metrics-layer[snowflake]`\n\nFor BigQuery run `pip install metrics-layer[bigquery]`\n\nFor Redshift run `pip install metrics-layer[redshift]`\n\n\n## Profile set up\n\nThere are several ways to set up a profile, we\'re going to look at the fastest one here.\n\nThe fastest way to get connected is to pass the necessary information directly into Metrics Layer. Once you\'ve installed the library with the warehouse you need, you should be able to run the code snippet below and start querying.\n\nYou\'ll pull the repo from Github for this example. For more detail on getting set up, check out the [documentation](https://docs.zenlytic.com)!\n\n\n```\nfrom metrics_layer import MetricsLayerConnection\n\n# Give metrics_layer the info to connect to your data model and warehouse\nconfig = {\n  "location": "https://myusername:myaccesstoken@github.com/myorg/myrepo.git",\n  "branch": "develop",\n  "connections": [\n    {\n      "name": "mycompany",              # The name of the connection in your data model (you\'ll see this in model files)\n      "type": "snowflake",\n      "account": "2e12ewdq.us-east-1",\n      "username": "demo_user",\n      "password": "q23e13erfwefqw",\n      "database": "ANALYTICS",\n      "schema": "DEV",                  # Optional\n    }\n  ],\n}\nconn = MetricsLayerConnection(**config)\n\n# You\'re off to the races. Query away!\ndf = conn.query(metrics=["total_revenue"], dimensions=["channel", "region"])\n```\n\nThat\'s it.\n\nFor more advanced methods of connection and more information about the project check out [the docs](https://docs.zenlytic.com).\n',
     'author': 'Paul Blankley',
     'author_email': 'paul@zenlytic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Zenlytic/metrics_layer',
```

### Comparing `metrics_layer-0.9.8/PKG-INFO` & `metrics_layer-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrics-layer
-Version: 0.9.8
+Version: 0.9.9
 Summary: The open source metrics layer.
 Home-page: https://github.com/Zenlytic/metrics_layer
 License: Apache 2.0
 Keywords: Metrics Layer,Looker,Analytics
 Author: Paul Blankley
 Author-email: paul@zenlytic.com
 Requires-Python: >=3.8.1,<3.10
```

