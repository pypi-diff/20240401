# Comparing `tmp/test_swagger_coverage-2.1.60.tar.gz` & `tmp/test_swagger_coverage-2.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_swagger_coverage-2.1.60.tar", max compression
+gzip compressed data, was "test_swagger_coverage-2.1.61.tar", max compression
```

## Comparing `test_swagger_coverage-2.1.60.tar` & `test_swagger_coverage-2.1.61.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-2.1.60/LICENSE
--rw-r--r--   0        0        0     5431 2024-04-01 12:14:21.892917 test_swagger_coverage-2.1.60/README.md
--rw-r--r--   0        0        0      667 2024-04-01 12:20:41.773571 test_swagger_coverage-2.1.60/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 08:08:13.320535 test_swagger_coverage-2.1.60/swagger_coverage/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-14 08:15:46.280403 test_swagger_coverage-2.1.60/swagger_coverage/scripts/swagger_report.py
--rw-r--r--   0        0        0        0 2023-04-30 12:36:25.778126 test_swagger_coverage-2.1.60/swagger_coverage/src/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-30 12:36:25.778625 test_swagger_coverage-2.1.60/swagger_coverage/src/check_data.py
--rw-r--r--   0        0        0     3509 2024-04-01 12:29:53.926522 test_swagger_coverage-2.1.60/swagger_coverage/src/coverage.py
--rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-2.1.60/swagger_coverage/src/deco.py
--rw-r--r--   0        0        0     2056 2023-04-30 12:36:25.779507 test_swagger_coverage-2.1.60/swagger_coverage/src/files.py
--rw-r--r--   0        0        0      849 2023-04-14 08:16:42.485998 test_swagger_coverage-2.1.60/swagger_coverage/src/logger.py
--rw-r--r--   0        0        0        0 2023-04-30 12:36:25.779568 test_swagger_coverage-2.1.60/swagger_coverage/src/models/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-30 12:36:25.779947 test_swagger_coverage-2.1.60/swagger_coverage/src/models/stats.py
--rw-r--r--   0        0        0      461 2023-04-30 12:36:25.780208 test_swagger_coverage-2.1.60/swagger_coverage/src/models/swagger_data.py
--rw-r--r--   0        0        0     2060 2023-04-30 12:36:25.780647 test_swagger_coverage-2.1.60/swagger_coverage/src/prepare_data.py
--rw-r--r--   0        0        0        0 2023-04-30 12:36:25.780712 test_swagger_coverage-2.1.60/swagger_coverage/src/report/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 12:36:25.780796 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/__init__.py
--rw-r--r--   0        0        0     6123 2023-04-30 12:36:25.781125 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/accordion.py
--rw-r--r--   0        0        0      883 2023-04-30 12:36:25.781388 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/body.py
--rw-r--r--   0        0        0      766 2023-04-30 12:36:25.781633 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/btn_group.py
--rw-r--r--   0        0        0      196 2023-04-30 12:36:25.781856 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/colors.py
--rw-r--r--   0        0        0      165 2023-04-30 12:36:25.782075 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/constants.py
--rw-r--r--   0        0        0      235 2023-04-30 12:36:25.782298 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/h2.py
--rw-r--r--   0        0        0      710 2023-04-30 12:36:25.782523 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/head.py
--rw-r--r--   0        0        0      180 2023-04-30 12:36:25.782931 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/href.py
--rw-r--r--   0        0        0     4706 2023-04-30 12:36:25.783274 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/html_report.py
--rw-r--r--   0        0        0      883 2023-04-30 12:36:25.783530 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/models.py
--rw-r--r--   0        0        0      670 2023-04-30 12:36:25.783844 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/navbar.py
--rw-r--r--   0        0        0      132 2023-04-30 12:36:25.784098 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/p.py
--rw-r--r--   0        0        0      446 2023-04-30 12:36:25.784331 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/prepare_data.py
--rw-r--r--   0        0        0      829 2023-04-30 12:36:25.784551 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/progress.py
--rw-r--r--   0        0        0     2911 2023-04-30 12:36:25.784797 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/scripts.py
--rw-r--r--   0        0        0     2027 2024-04-01 12:14:21.898733 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/table.py
--rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785160 test_swagger_coverage-2.1.60/swagger_coverage/src/report/plain/__init__.py
--rw-r--r--   0        0        0       64 2023-04-30 12:36:25.785426 test_swagger_coverage-2.1.60/swagger_coverage/src/report/plain/plain_report.py
--rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785482 test_swagger_coverage-2.1.60/swagger_coverage/src/report/report.py
--rw-r--r--   0        0        0      902 2024-04-01 12:25:52.030546 test_swagger_coverage-2.1.60/swagger_coverage/src/requests.py
--rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785764 test_swagger_coverage-2.1.60/swagger_coverage/src/results/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-30 12:36:25.786131 test_swagger_coverage-2.1.60/swagger_coverage/src/results/load_results.py
--rw-r--r--   0        0        0      550 2023-04-30 12:36:25.786355 test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_diff.py
--rw-r--r--   0        0        0     1470 2023-04-30 12:36:25.786585 test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_results.py
--rw-r--r--   0        0        0     2907 2023-04-30 12:36:25.786828 test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_summary.py
--rw-r--r--   0        0        0      326 2023-04-14 12:08:09.802242 test_swagger_coverage-2.1.60/swagger_coverage/src/singltone_like.py
--rw-r--r--   0        0        0      384 2023-04-30 12:36:25.787116 test_swagger_coverage-2.1.60/swagger_coverage/src/utils.py
--rw-r--r--   0        0        0     6118 1970-01-01 00:00:00.000000 test_swagger_coverage-2.1.60/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-2.1.61/LICENSE
+-rw-r--r--   0        0        0     5431 2024-04-01 12:14:21.892917 test_swagger_coverage-2.1.61/README.md
+-rw-r--r--   0        0        0      667 2024-04-01 14:50:46.903248 test_swagger_coverage-2.1.61/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 08:08:13.320535 test_swagger_coverage-2.1.61/swagger_coverage/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-14 08:15:46.280403 test_swagger_coverage-2.1.61/swagger_coverage/scripts/swagger_report.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.778126 test_swagger_coverage-2.1.61/swagger_coverage/src/__init__.py
+-rw-r--r--   0        0        0     1354 2023-04-30 12:36:25.778625 test_swagger_coverage-2.1.61/swagger_coverage/src/check_data.py
+-rw-r--r--   0        0        0     3467 2024-04-01 14:50:40.765627 test_swagger_coverage-2.1.61/swagger_coverage/src/coverage.py
+-rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-2.1.61/swagger_coverage/src/deco.py
+-rw-r--r--   0        0        0     2056 2023-04-30 12:36:25.779507 test_swagger_coverage-2.1.61/swagger_coverage/src/files.py
+-rw-r--r--   0        0        0      849 2023-04-14 08:16:42.485998 test_swagger_coverage-2.1.61/swagger_coverage/src/logger.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.779568 test_swagger_coverage-2.1.61/swagger_coverage/src/models/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-30 12:36:25.779947 test_swagger_coverage-2.1.61/swagger_coverage/src/models/stats.py
+-rw-r--r--   0        0        0      461 2023-04-30 12:36:25.780208 test_swagger_coverage-2.1.61/swagger_coverage/src/models/swagger_data.py
+-rw-r--r--   0        0        0     2060 2023-04-30 12:36:25.780647 test_swagger_coverage-2.1.61/swagger_coverage/src/prepare_data.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.780712 test_swagger_coverage-2.1.61/swagger_coverage/src/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.780796 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/__init__.py
+-rw-r--r--   0        0        0     6123 2023-04-30 12:36:25.781125 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/accordion.py
+-rw-r--r--   0        0        0      883 2023-04-30 12:36:25.781388 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/body.py
+-rw-r--r--   0        0        0      766 2023-04-30 12:36:25.781633 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/btn_group.py
+-rw-r--r--   0        0        0      196 2023-04-30 12:36:25.781856 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/colors.py
+-rw-r--r--   0        0        0      165 2023-04-30 12:36:25.782075 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/constants.py
+-rw-r--r--   0        0        0      235 2023-04-30 12:36:25.782298 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/h2.py
+-rw-r--r--   0        0        0      710 2023-04-30 12:36:25.782523 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/head.py
+-rw-r--r--   0        0        0      180 2023-04-30 12:36:25.782931 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/href.py
+-rw-r--r--   0        0        0     4706 2023-04-30 12:36:25.783274 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/html_report.py
+-rw-r--r--   0        0        0      883 2023-04-30 12:36:25.783530 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/models.py
+-rw-r--r--   0        0        0      670 2023-04-30 12:36:25.783844 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/navbar.py
+-rw-r--r--   0        0        0      132 2023-04-30 12:36:25.784098 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/p.py
+-rw-r--r--   0        0        0      446 2023-04-30 12:36:25.784331 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/prepare_data.py
+-rw-r--r--   0        0        0      829 2023-04-30 12:36:25.784551 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/progress.py
+-rw-r--r--   0        0        0     2911 2023-04-30 12:36:25.784797 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/scripts.py
+-rw-r--r--   0        0        0     2027 2024-04-01 12:14:21.898733 test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/table.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785160 test_swagger_coverage-2.1.61/swagger_coverage/src/report/plain/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-30 12:36:25.785426 test_swagger_coverage-2.1.61/swagger_coverage/src/report/plain/plain_report.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785482 test_swagger_coverage-2.1.61/swagger_coverage/src/report/report.py
+-rw-r--r--   0        0        0      902 2024-04-01 14:50:25.375719 test_swagger_coverage-2.1.61/swagger_coverage/src/requests.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785764 test_swagger_coverage-2.1.61/swagger_coverage/src/results/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-30 12:36:25.786131 test_swagger_coverage-2.1.61/swagger_coverage/src/results/load_results.py
+-rw-r--r--   0        0        0      550 2023-04-30 12:36:25.786355 test_swagger_coverage-2.1.61/swagger_coverage/src/results/swagger_diff.py
+-rw-r--r--   0        0        0     1470 2023-04-30 12:36:25.786585 test_swagger_coverage-2.1.61/swagger_coverage/src/results/swagger_results.py
+-rw-r--r--   0        0        0     2907 2023-04-30 12:36:25.786828 test_swagger_coverage-2.1.61/swagger_coverage/src/results/swagger_summary.py
+-rw-r--r--   0        0        0      326 2023-04-14 12:08:09.802242 test_swagger_coverage-2.1.61/swagger_coverage/src/singltone_like.py
+-rw-r--r--   0        0        0      384 2023-04-30 12:36:25.787116 test_swagger_coverage-2.1.61/swagger_coverage/src/utils.py
+-rw-r--r--   0        0        0     6118 1970-01-01 00:00:00.000000 test_swagger_coverage-2.1.61/PKG-INFO
```

### Comparing `test_swagger_coverage-2.1.60/LICENSE` & `test_swagger_coverage-2.1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/README.md` & `test_swagger_coverage-2.1.61/README.md`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/pyproject.toml` & `test_swagger_coverage-2.1.61/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-swagger-coverage"
-version = "2.1.60"
+version = "2.1.61"
 description = "Swagger coverage for API tests"
 authors = ["alexanderlozovoy <berpress@gmail.com>"]
 packages = [{ include = "swagger_coverage" }]
 readme = "README.md"
 repository = "https://github.com/berpress/swagger-coverage"
 
 [tool.poetry.dependencies]
```

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/scripts/swagger_report.py` & `test_swagger_coverage-2.1.61/swagger_coverage/scripts/swagger_report.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/check_data.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/check_data.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/coverage.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/coverage.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,20 +61,20 @@
             prepare = PrepareData()
             prepare_data = prepare.prepare_swagger_data(
                 data=load_data, status_codes=self.status_codes
             )
             save_yaml(path_file=self.path_to_file, data=prepare_data)
         self._prepare_exist_swagger()
 
-    def _select_urls(self, url: str, urls: str) -> List[str]:
+    def _select_urls(self, url: str, urls: str):
         if url:
             return [url]
         if len(urls) > 0:
             return urls
-        raise ValueError("Add swagger url/urls")
+        return None
 
     def _prepare_exist_swagger(self):
         dict_data = load_yaml(path_to_file=self.path_to_file)
         prepare = PrepareData()
         self.data.swagger_data = prepare.prepare_check_file_data(dict_data)
 
     def save_results(self) -> str:
```

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/deco.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/deco.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/files.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/files.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/logger.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/logger.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/models/stats.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/models/stats.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/prepare_data.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/prepare_data.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/accordion.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/accordion.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/body.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/body.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/btn_group.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/btn_group.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/head.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/head.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/html_report.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/html_report.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/models.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/models.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/navbar.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/navbar.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/progress.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/progress.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/scripts.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/scripts.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/table.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/report/html/table.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/requests.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/requests.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/results/load_results.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/results/load_results.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_diff.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/results/swagger_diff.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_results.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/results/swagger_results.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_summary.py` & `test_swagger_coverage-2.1.61/swagger_coverage/src/results/swagger_summary.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.60/PKG-INFO` & `test_swagger_coverage-2.1.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-swagger-coverage
-Version: 2.1.60
+Version: 2.1.61
 Summary: Swagger coverage for API tests
 Home-page: https://github.com/berpress/swagger-coverage
 Author: alexanderlozovoy
 Author-email: berpress@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

