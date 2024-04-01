# Comparing `tmp/test_swagger_coverage-2.1.59.tar.gz` & `tmp/test_swagger_coverage-2.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_swagger_coverage-2.1.59.tar", max compression
+gzip compressed data, was "test_swagger_coverage-2.1.60.tar", max compression
```

## Comparing `test_swagger_coverage-2.1.59.tar` & `test_swagger_coverage-2.1.60.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-2.1.59/LICENSE
--rw-r--r--   0        0        0     5418 2023-04-30 10:05:22.859355 test_swagger_coverage-2.1.59/README.md
--rw-r--r--   0        0        0      667 2023-04-30 10:55:24.027848 test_swagger_coverage-2.1.59/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 08:08:13.320535 test_swagger_coverage-2.1.59/swagger_coverage/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-14 08:15:46.280403 test_swagger_coverage-2.1.59/swagger_coverage/scripts/swagger_report.py
--rw-r--r--   0        0        0        0 2023-04-14 08:08:31.328063 test_swagger_coverage-2.1.59/swagger_coverage/src/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-14 13:05:24.138537 test_swagger_coverage-2.1.59/swagger_coverage/src/check_data.py
--rw-r--r--   0        0        0     3225 2023-04-30 10:51:59.096355 test_swagger_coverage-2.1.59/swagger_coverage/src/coverage.py
--rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-2.1.59/swagger_coverage/src/deco.py
--rw-r--r--   0        0        0     2056 2023-04-27 16:02:40.028529 test_swagger_coverage-2.1.59/swagger_coverage/src/files.py
--rw-r--r--   0        0        0      849 2023-04-14 08:16:42.485998 test_swagger_coverage-2.1.59/swagger_coverage/src/logger.py
--rw-r--r--   0        0        0        0 2023-04-14 11:31:54.617585 test_swagger_coverage-2.1.59/swagger_coverage/src/models/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-27 16:01:57.068459 test_swagger_coverage-2.1.59/swagger_coverage/src/models/stats.py
--rw-r--r--   0        0        0      461 2023-04-27 14:54:00.916774 test_swagger_coverage-2.1.59/swagger_coverage/src/models/swagger_data.py
--rw-r--r--   0        0        0     2060 2023-04-27 16:24:53.724437 test_swagger_coverage-2.1.59/swagger_coverage/src/prepare_data.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:27.954717 test_swagger_coverage-2.1.59/swagger_coverage/src/report/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:45.222122 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/__init__.py
--rw-r--r--   0        0        0     6123 2023-04-27 16:03:56.022244 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/accordion.py
--rw-r--r--   0        0        0      883 2023-04-27 16:03:26.744052 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/body.py
--rw-r--r--   0        0        0      766 2023-04-27 16:03:55.974209 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/btn_group.py
--rw-r--r--   0        0        0      196 2023-04-27 16:01:57.073937 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/colors.py
--rw-r--r--   0        0        0      165 2023-04-27 16:01:57.076766 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/constants.py
--rw-r--r--   0        0        0      235 2023-04-27 16:01:57.084743 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/h2.py
--rw-r--r--   0        0        0      710 2023-04-27 16:03:55.971852 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/head.py
--rw-r--r--   0        0        0      180 2023-04-27 16:01:57.092106 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/href.py
--rw-r--r--   0        0        0     4706 2023-04-30 07:05:11.452022 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/html_report.py
--rw-r--r--   0        0        0      883 2023-04-27 16:01:57.123593 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/models.py
--rw-r--r--   0        0        0      670 2023-04-27 16:03:54.865325 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/navbar.py
--rw-r--r--   0        0        0      132 2023-04-27 16:01:57.095766 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/p.py
--rw-r--r--   0        0        0      446 2023-04-27 16:01:57.121785 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/prepare_data.py
--rw-r--r--   0        0        0      829 2023-04-27 16:06:14.093094 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/progress.py
--rw-r--r--   0        0        0     2911 2023-04-27 16:01:57.330789 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/scripts.py
--rw-r--r--   0        0        0     2027 2023-04-30 09:13:46.596899 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/table.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:38.904729 test_swagger_coverage-2.1.59/swagger_coverage/src/report/plain/__init__.py
--rw-r--r--   0        0        0       64 2023-04-27 16:01:57.115041 test_swagger_coverage-2.1.59/swagger_coverage/src/report/plain/plain_report.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:33.654900 test_swagger_coverage-2.1.59/swagger_coverage/src/report/report.py
--rw-r--r--   0        0        0      710 2023-04-30 08:39:24.664235 test_swagger_coverage-2.1.59/swagger_coverage/src/requests.py
--rw-r--r--   0        0        0        0 2023-04-17 15:15:04.775886 test_swagger_coverage-2.1.59/swagger_coverage/src/results/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-27 16:19:19.207957 test_swagger_coverage-2.1.59/swagger_coverage/src/results/load_results.py
--rw-r--r--   0        0        0      550 2023-04-27 16:01:57.133390 test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_diff.py
--rw-r--r--   0        0        0     1470 2023-04-27 16:05:14.499393 test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_results.py
--rw-r--r--   0        0        0     2907 2023-04-27 16:05:09.299861 test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_summary.py
--rw-r--r--   0        0        0      326 2023-04-14 12:08:09.802242 test_swagger_coverage-2.1.59/swagger_coverage/src/singltone_like.py
--rw-r--r--   0        0        0      384 2023-04-27 16:01:57.142956 test_swagger_coverage-2.1.59/swagger_coverage/src/utils.py
--rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 test_swagger_coverage-2.1.59/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-2.1.60/LICENSE
+-rw-r--r--   0        0        0     5431 2024-04-01 12:14:21.892917 test_swagger_coverage-2.1.60/README.md
+-rw-r--r--   0        0        0      667 2024-04-01 12:20:41.773571 test_swagger_coverage-2.1.60/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 08:08:13.320535 test_swagger_coverage-2.1.60/swagger_coverage/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-14 08:15:46.280403 test_swagger_coverage-2.1.60/swagger_coverage/scripts/swagger_report.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.778126 test_swagger_coverage-2.1.60/swagger_coverage/src/__init__.py
+-rw-r--r--   0        0        0     1354 2023-04-30 12:36:25.778625 test_swagger_coverage-2.1.60/swagger_coverage/src/check_data.py
+-rw-r--r--   0        0        0     3509 2024-04-01 12:29:53.926522 test_swagger_coverage-2.1.60/swagger_coverage/src/coverage.py
+-rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-2.1.60/swagger_coverage/src/deco.py
+-rw-r--r--   0        0        0     2056 2023-04-30 12:36:25.779507 test_swagger_coverage-2.1.60/swagger_coverage/src/files.py
+-rw-r--r--   0        0        0      849 2023-04-14 08:16:42.485998 test_swagger_coverage-2.1.60/swagger_coverage/src/logger.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.779568 test_swagger_coverage-2.1.60/swagger_coverage/src/models/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-30 12:36:25.779947 test_swagger_coverage-2.1.60/swagger_coverage/src/models/stats.py
+-rw-r--r--   0        0        0      461 2023-04-30 12:36:25.780208 test_swagger_coverage-2.1.60/swagger_coverage/src/models/swagger_data.py
+-rw-r--r--   0        0        0     2060 2023-04-30 12:36:25.780647 test_swagger_coverage-2.1.60/swagger_coverage/src/prepare_data.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.780712 test_swagger_coverage-2.1.60/swagger_coverage/src/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.780796 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/__init__.py
+-rw-r--r--   0        0        0     6123 2023-04-30 12:36:25.781125 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/accordion.py
+-rw-r--r--   0        0        0      883 2023-04-30 12:36:25.781388 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/body.py
+-rw-r--r--   0        0        0      766 2023-04-30 12:36:25.781633 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/btn_group.py
+-rw-r--r--   0        0        0      196 2023-04-30 12:36:25.781856 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/colors.py
+-rw-r--r--   0        0        0      165 2023-04-30 12:36:25.782075 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/constants.py
+-rw-r--r--   0        0        0      235 2023-04-30 12:36:25.782298 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/h2.py
+-rw-r--r--   0        0        0      710 2023-04-30 12:36:25.782523 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/head.py
+-rw-r--r--   0        0        0      180 2023-04-30 12:36:25.782931 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/href.py
+-rw-r--r--   0        0        0     4706 2023-04-30 12:36:25.783274 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/html_report.py
+-rw-r--r--   0        0        0      883 2023-04-30 12:36:25.783530 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/models.py
+-rw-r--r--   0        0        0      670 2023-04-30 12:36:25.783844 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/navbar.py
+-rw-r--r--   0        0        0      132 2023-04-30 12:36:25.784098 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/p.py
+-rw-r--r--   0        0        0      446 2023-04-30 12:36:25.784331 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/prepare_data.py
+-rw-r--r--   0        0        0      829 2023-04-30 12:36:25.784551 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/progress.py
+-rw-r--r--   0        0        0     2911 2023-04-30 12:36:25.784797 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/scripts.py
+-rw-r--r--   0        0        0     2027 2024-04-01 12:14:21.898733 test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/table.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785160 test_swagger_coverage-2.1.60/swagger_coverage/src/report/plain/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-30 12:36:25.785426 test_swagger_coverage-2.1.60/swagger_coverage/src/report/plain/plain_report.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785482 test_swagger_coverage-2.1.60/swagger_coverage/src/report/report.py
+-rw-r--r--   0        0        0      902 2024-04-01 12:25:52.030546 test_swagger_coverage-2.1.60/swagger_coverage/src/requests.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:36:25.785764 test_swagger_coverage-2.1.60/swagger_coverage/src/results/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-30 12:36:25.786131 test_swagger_coverage-2.1.60/swagger_coverage/src/results/load_results.py
+-rw-r--r--   0        0        0      550 2023-04-30 12:36:25.786355 test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_diff.py
+-rw-r--r--   0        0        0     1470 2023-04-30 12:36:25.786585 test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_results.py
+-rw-r--r--   0        0        0     2907 2023-04-30 12:36:25.786828 test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_summary.py
+-rw-r--r--   0        0        0      326 2023-04-14 12:08:09.802242 test_swagger_coverage-2.1.60/swagger_coverage/src/singltone_like.py
+-rw-r--r--   0        0        0      384 2023-04-30 12:36:25.787116 test_swagger_coverage-2.1.60/swagger_coverage/src/utils.py
+-rw-r--r--   0        0        0     6118 1970-01-01 00:00:00.000000 test_swagger_coverage-2.1.60/PKG-INFO
```

### Comparing `test_swagger_coverage-2.1.59/LICENSE` & `test_swagger_coverage-2.1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/README.md` & `test_swagger_coverage-2.1.60/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: test-swagger-coverage
+Version: 2.1.60
+Summary: Swagger coverage for API tests
+Home-page: https://github.com/berpress/swagger-coverage
+Author: alexanderlozovoy
+Author-email: berpress@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Repository, https://github.com/berpress/swagger-coverage
+Description-Content-Type: text/markdown
+
 # swagger-coverage
 [![Tests](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml/badge.svg)](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml)
 ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/maintainability)](https://codeclimate.com/github/berpress/swagger-coverage/maintainability)
 [![PyPI version](https://badge.fury.io/py/test-swagger-coverage.svg)](https://badge.fury.io/py/test-swagger-coverage)
 [![Downloads](https://pepy.tech/badge/test-swagger-coverage)](https://pepy.tech/project/test-swagger-coverage)
 
 About
 ------------
 
 Swagger coverage report helps the QA automation and developer to get a simple API coverage report for endpoints tests
 
-![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_report_2.png)
+![](https://github.com/berpress/python-api-tests/blob/main/images/1.png?raw=true)
 
 Installation
 ------------
 
 You can install ``test-swagger-coverage`` via `pip`_ from `PyPI`_::
 
     $ pip install test-swagger-coverage
@@ -65,86 +83,106 @@
   statuses:
   - 200
   - 404
   tag: pet
   ...
  ```
 
-where **regUser** is the unique id of our endpoint
+where **addPet** is the unique id of our endpoint
+
+ ```
+ ...
+addPet:
+  description: 'Add new pet'
+  method: POST
+  path: /pet
+  statuses:
+  - 200
+  - 404  <---- add 404 status code 
+  - 404
+  tag: pet
+  ...
+ ```
+
+We can change or add our data, for example, a new status code, which will need to be checked
 
 **statuses** is a list of statuses that we will check (that they were called).
 You can customize this list yourself.
 
-Only we will check 201 status, as described in the user registration swagger. So I will add it.
 
 
 Let's create a simple test and build a report. For requests, you will use the **requests** library.
+We will check that a non-existent pet returns a 404 status code
 
 ```python
 import requests
+
 from swagger_coverage.src.coverage import SwaggerCoverage
 from swagger_coverage.src.deco import swagger
 
-# swagger data preparation
-swagger_url = "https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0"
-api_url = "https://api.swaggerhub.com/apis/"
-path='/report' # path to swagger coverage report
-swagger_rep = SwaggerCoverage(api_url=api_url, url=swagger_url, path=path)
-swagger_rep.create_coverage_data()
-
-
-# function to call a request to the server
-@swagger("regUser")
-def register_user(payload: dict):
-    return requests.post('https://stores-tests-api.herokuapp.com/register',
-                         json=payload)
-
-
-# test
-data = {"username": "test2023@test.com", "password": "Password"}
-response = register_user(data)
-assert response.status_code == 201
+# settings
+SWAGGER_URL = 'https://petstore.swagger.io/v2/swagger.json'
+STATUS_CODES = [200, 404]
+
+
+# our request that we will cover
+@swagger("getPetById")
+def get_pet_by_id():
+    return requests.get("https://petstore.swagger.io/v2/pet/999")  # <-- 999 pet id no such exists
+
+
+# create swagger objects
+swagger = SwaggerCoverage(
+    url=SWAGGER_URL,
+    status_codes=STATUS_CODES,
+    api_url="https://petstore.swagger.io/",
+)
+swagger.create_coverage_data()
+get_pet_by_id()
+swagger.create_report()
 
-# create report
-swagger_rep.create_report()
 
 ```
 **swagger data preparation**: Prepare our file data_swagger.yaml, it will be created automatically.
 
-**function to call a request to the server**:  We will write a user registration call. Declaring a function with a decorator **@swagger("regUser")**.
-**"regUser"** taken from file **data_swagger.yaml**, this is unique id of our endpoint.
+**function to call a request to the server**:  We will write a get pet by id call. Declaring a function with a decorator **@swagger("getPetById")**.
+**"getPetById"** taken from file **data_swagger.yaml**, this is unique id of our endpoint.
 
-**test**: run the test
+**get_pet_by_id**: run the test (our request)
 
 **create report**: create a report.
 
 
 After that, in the folder **swagger_report** we will receive a report **index.html**.
 
 Let's see it
 
-![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_register.png)
+![](https://github.com/berpress/python-api-tests/blob/main/images/4.png?raw=true)
+
+As you can see, an endpoint appeared in the report, which was partially verified. Filtering the results and open more info window
+
+![](https://github.com/berpress/python-api-tests/blob/main/images/5.png?raw=true)
+
+Test and coverage passed successfully!
 
-As you can see, we have increased the counter of verified endpoints
 
 If you use **pytest**, add this code in conftest.py
 
 ```python
+import pytest
+from swagger_coverage.src.coverage import SwaggerCoverage
+
 @pytest.fixture(scope="session", autouse=True)
 def swagger_checker(request):
-    url = request.config.getoption("--swagger-url")
-    url_api = request.config.getoption("--api-url")
-    path = '/report'
-    swagger = SwaggerCoverage(api_url=url_api, url=url, path=path)
+    url = 'https://petstore.swagger.io/v2/swagger.json'
+    url_api = 'https://petstore.swagger.io'
+    swagger = SwaggerCoverage(api_url=url_api, url=url)
     swagger.create_coverage_data()
     yield
     swagger.create_report()
 ```
 Also, at the end of the report, you can find a table of average request times for routes
-![](https://github.com/berpress/python-api-tests/blob/main/images/requets_time.png?raw=true)
-
-
-Also, at the end of the report, you can find a table of average request times for routes
 
 More example with pytest and API tests https://github.com/berpress/python-api-tests
 
-Report example [https://github.com/berpress/python-api-tests/tree/main/swagger_report](https://github.com/berpress/python-api-tests/tree/main/report)
+Report example https://github.com/berpress/python-api-tests/blob/main/swagger_report/index.html
+
```

### Comparing `test_swagger_coverage-2.1.59/pyproject.toml` & `test_swagger_coverage-2.1.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-swagger-coverage"
-version = "2.1.59"
+version = "2.1.60"
 description = "Swagger coverage for API tests"
 authors = ["alexanderlozovoy <berpress@gmail.com>"]
 packages = [{ include = "swagger_coverage" }]
 readme = "README.md"
 repository = "https://github.com/berpress/swagger-coverage"
 
 [tool.poetry.dependencies]
```

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/scripts/swagger_report.py` & `test_swagger_coverage-2.1.60/swagger_coverage/scripts/swagger_report.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/check_data.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/check_data.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/coverage.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/coverage.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 _TEST_SWAGGER_FILE_NAME = "data_swagger.yaml"
 _SWAGGER_REPORT_DIR = "swagger_report"
 _DEFAULT_STATUS_CODE = [200, 400, 401, 403]
 
 
 class SwaggerCoverage(metaclass=Singleton):
     def __init__(
-        self,
-        url: str = None,
-        api_url: str = None,
-        status_codes: List[int] = None,
-        path: str = _SWAGGER_REPORT_DIR,
+            self,
+            url: str = None,
+            urls: List[str] = None,
+            api_url: str = None,
+            status_codes: List[int] = None,
+            path: str = _SWAGGER_REPORT_DIR,
     ):
         """
         :param url: Swagger url, example https://petstore.swagger.io/v2/swagger.json # noqa
         :param api_url: Api url, example https://petstore3.swagger.io/
         :param status_codes: List off status codes, example [200, 400]
         :param path: path to
         """
-        self.swagger_url = url
+        self.swagger_url = self._select_urls(url, urls)
         self.api_url = api_url
         if status_codes is None:
             self.status_codes = _DEFAULT_STATUS_CODE
         else:
             self.status_codes = [int(s) for s in status_codes]
         self.path = prepare_path(path=path, report_dir=_SWAGGER_REPORT_DIR)
         self.data = SwaggerData()
@@ -60,14 +61,21 @@
             prepare = PrepareData()
             prepare_data = prepare.prepare_swagger_data(
                 data=load_data, status_codes=self.status_codes
             )
             save_yaml(path_file=self.path_to_file, data=prepare_data)
         self._prepare_exist_swagger()
 
+    def _select_urls(self, url: str, urls: str) -> List[str]:
+        if url:
+            return [url]
+        if len(urls) > 0:
+            return urls
+        raise ValueError("Add swagger url/urls")
+
     def _prepare_exist_swagger(self):
         dict_data = load_yaml(path_to_file=self.path_to_file)
         prepare = PrepareData()
         self.data.swagger_data = prepare.prepare_check_file_data(dict_data)
 
     def save_results(self) -> str:
         results = SwaggerResults(self)
```

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/deco.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/deco.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/files.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/files.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/logger.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/logger.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/models/stats.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/models/stats.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/prepare_data.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/prepare_data.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/accordion.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/accordion.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/body.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/body.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/btn_group.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/btn_group.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/head.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/head.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/html_report.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/html_report.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/models.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/models.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/navbar.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/navbar.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/progress.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/progress.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/scripts.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/scripts.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/table.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/report/html/table.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/results/load_results.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/results/load_results.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_diff.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_diff.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_results.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_results.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_summary.py` & `test_swagger_coverage-2.1.60/swagger_coverage/src/results/swagger_summary.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.59/PKG-INFO` & `test_swagger_coverage-2.1.60/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-Metadata-Version: 2.1
-Name: test-swagger-coverage
-Version: 2.1.59
-Summary: Swagger coverage for API tests
-Home-page: https://github.com/berpress/swagger-coverage
-Author: alexanderlozovoy
-Author-email: berpress@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Project-URL: Repository, https://github.com/berpress/swagger-coverage
-Description-Content-Type: text/markdown
-
 # swagger-coverage
 [![Tests](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml/badge.svg)](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml)
 ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/maintainability)](https://codeclimate.com/github/berpress/swagger-coverage/maintainability)
 [![PyPI version](https://badge.fury.io/py/test-swagger-coverage.svg)](https://badge.fury.io/py/test-swagger-coverage)
 [![Downloads](https://pepy.tech/badge/test-swagger-coverage)](https://pepy.tech/project/test-swagger-coverage)
 
 About
 ------------
 
 Swagger coverage report helps the QA automation and developer to get a simple API coverage report for endpoints tests
 
-![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_report_2.png)
+![](https://github.com/berpress/python-api-tests/blob/main/images/1.png?raw=true)
 
 Installation
 ------------
 
 You can install ``test-swagger-coverage`` via `pip`_ from `PyPI`_::
 
     $ pip install test-swagger-coverage
@@ -83,87 +65,105 @@
   statuses:
   - 200
   - 404
   tag: pet
   ...
  ```
 
-where **regUser** is the unique id of our endpoint
+where **addPet** is the unique id of our endpoint
+
+ ```
+ ...
+addPet:
+  description: 'Add new pet'
+  method: POST
+  path: /pet
+  statuses:
+  - 200
+  - 404  <---- add 404 status code 
+  - 404
+  tag: pet
+  ...
+ ```
+
+We can change or add our data, for example, a new status code, which will need to be checked
 
 **statuses** is a list of statuses that we will check (that they were called).
 You can customize this list yourself.
 
-Only we will check 201 status, as described in the user registration swagger. So I will add it.
 
 
 Let's create a simple test and build a report. For requests, you will use the **requests** library.
+We will check that a non-existent pet returns a 404 status code
 
 ```python
 import requests
+
 from swagger_coverage.src.coverage import SwaggerCoverage
 from swagger_coverage.src.deco import swagger
 
-# swagger data preparation
-swagger_url = "https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0"
-api_url = "https://api.swaggerhub.com/apis/"
-path='/report' # path to swagger coverage report
-swagger_rep = SwaggerCoverage(api_url=api_url, url=swagger_url, path=path)
-swagger_rep.create_coverage_data()
-
-
-# function to call a request to the server
-@swagger("regUser")
-def register_user(payload: dict):
-    return requests.post('https://stores-tests-api.herokuapp.com/register',
-                         json=payload)
-
-
-# test
-data = {"username": "test2023@test.com", "password": "Password"}
-response = register_user(data)
-assert response.status_code == 201
+# settings
+SWAGGER_URL = 'https://petstore.swagger.io/v2/swagger.json'
+STATUS_CODES = [200, 404]
+
+
+# our request that we will cover
+@swagger("getPetById")
+def get_pet_by_id():
+    return requests.get("https://petstore.swagger.io/v2/pet/999")  # <-- 999 pet id no such exists
+
+
+# create swagger objects
+swagger = SwaggerCoverage(
+    url=SWAGGER_URL,
+    status_codes=STATUS_CODES,
+    api_url="https://petstore.swagger.io/",
+)
+swagger.create_coverage_data()
+get_pet_by_id()
+swagger.create_report()
 
-# create report
-swagger_rep.create_report()
 
 ```
 **swagger data preparation**: Prepare our file data_swagger.yaml, it will be created automatically.
 
-**function to call a request to the server**:  We will write a user registration call. Declaring a function with a decorator **@swagger("regUser")**.
-**"regUser"** taken from file **data_swagger.yaml**, this is unique id of our endpoint.
+**function to call a request to the server**:  We will write a get pet by id call. Declaring a function with a decorator **@swagger("getPetById")**.
+**"getPetById"** taken from file **data_swagger.yaml**, this is unique id of our endpoint.
 
-**test**: run the test
+**get_pet_by_id**: run the test (our request)
 
 **create report**: create a report.
 
 
 After that, in the folder **swagger_report** we will receive a report **index.html**.
 
 Let's see it
 
-![](https://github.com/berpress/python-api-tests/blob/main/images/swagger_register.png)
+![](https://github.com/berpress/python-api-tests/blob/main/images/4.png?raw=true)
+
+As you can see, an endpoint appeared in the report, which was partially verified. Filtering the results and open more info window
+
+![](https://github.com/berpress/python-api-tests/blob/main/images/5.png?raw=true)
+
+Test and coverage passed successfully!
 
-As you can see, we have increased the counter of verified endpoints
 
 If you use **pytest**, add this code in conftest.py
 
 ```python
+import pytest
+from swagger_coverage.src.coverage import SwaggerCoverage
+
 @pytest.fixture(scope="session", autouse=True)
 def swagger_checker(request):
-    url = request.config.getoption("--swagger-url")
-    url_api = request.config.getoption("--api-url")
-    path = '/report'
-    swagger = SwaggerCoverage(api_url=url_api, url=url, path=path)
+    url = 'https://petstore.swagger.io/v2/swagger.json'
+    url_api = 'https://petstore.swagger.io'
+    swagger = SwaggerCoverage(api_url=url_api, url=url)
     swagger.create_coverage_data()
     yield
     swagger.create_report()
 ```
 Also, at the end of the report, you can find a table of average request times for routes
-![](https://github.com/berpress/python-api-tests/blob/main/images/requets_time.png?raw=true)
-
-
-Also, at the end of the report, you can find a table of average request times for routes
 
 More example with pytest and API tests https://github.com/berpress/python-api-tests
 
-Report example [https://github.com/berpress/python-api-tests/tree/main/swagger_report](https://github.com/berpress/python-api-tests/tree/main/report)
-
+Report example https://github.com/berpress/python-api-tests/blob/main/swagger_report/index.html
```

