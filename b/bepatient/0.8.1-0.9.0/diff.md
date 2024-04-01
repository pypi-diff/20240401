# Comparing `tmp/bepatient-0.8.1.tar.gz` & `tmp/bepatient-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bepatient-0.8.1.tar", last modified: Sun Dec 10 18:11:20 2023, max compression
+gzip compressed data, was "bepatient-0.9.0.tar", last modified: Mon Mar  4 19:33:47 2024, max compression
```

## Comparing `bepatient-0.8.1.tar` & `bepatient-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.041665 bepatient-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-10 18:11:06.000000 bepatient-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2023-12-10 18:11:20.041665 bepatient-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2023-12-10 18:11:06.000000 bepatient-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.033665 bepatient-0.8.1/bepatient/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/curler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.037665 bepatient-0.8.1/bepatient/waiter_src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.037665 bepatient-0.8.1/bepatient/waiter_src/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/checkers/response_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/comparators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.037665 bepatient-0.8.1/bepatient/waiter_src/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/exceptions/executor_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/exceptions/waiter_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.037665 bepatient-0.8.1/bepatient/waiter_src/executors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/executors/requests_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-12-10 18:11:06.000000 bepatient-0.8.1/bepatient/waiter_src/waiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.037665 bepatient-0.8.1/bepatient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2023-12-10 18:11:20.000000 bepatient-0.8.1/bepatient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-12-10 18:11:20.000000 bepatient-0.8.1/bepatient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 18:11:20.000000 bepatient-0.8.1/bepatient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-10 18:11:20.000000 bepatient-0.8.1/bepatient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-10 18:11:20.000000 bepatient-0.8.1/bepatient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2023-12-10 18:11:06.000000 bepatient-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-12-10 18:11:20.041665 bepatient-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-10 18:11:06.000000 bepatient-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 18:11:20.037665 bepatient-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    28396 2023-12-10 18:11:06.000000 bepatient-0.8.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2023-12-10 18:11:06.000000 bepatient-0.8.1/tests/test_curler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2023-12-10 18:11:06.000000 bepatient-0.8.1/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.846812 bepatient-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-04 19:33:40.000000 bepatient-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-03-04 19:33:47.846812 bepatient-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-03-04 19:33:40.000000 bepatient-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.842812 bepatient-0.9.0/bepatient/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/curler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.842812 bepatient-0.9.0/bepatient/waiter_src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.842812 bepatient-0.9.0/bepatient/waiter_src/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/checkers/response_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/comparators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.842812 bepatient-0.9.0/bepatient/waiter_src/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/exceptions/executor_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/exceptions/waiter_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.842812 bepatient-0.9.0/bepatient/waiter_src/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/executors/requests_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-04 19:33:40.000000 bepatient-0.9.0/bepatient/waiter_src/waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.846812 bepatient-0.9.0/bepatient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-03-04 19:33:47.000000 bepatient-0.9.0/bepatient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-04 19:33:47.000000 bepatient-0.9.0/bepatient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 19:33:47.000000 bepatient-0.9.0/bepatient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-04 19:33:47.000000 bepatient-0.9.0/bepatient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 19:33:47.000000 bepatient-0.9.0/bepatient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-04 19:33:40.000000 bepatient-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-04 19:33:47.846812 bepatient-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-04 19:33:40.000000 bepatient-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:33:47.846812 bepatient-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    28792 2024-03-04 19:33:40.000000 bepatient-0.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-04 19:33:40.000000 bepatient-0.9.0/tests/test_curler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-04 19:33:40.000000 bepatient-0.9.0/tests/test_e2e.py
```

### Comparing `bepatient-0.8.1/LICENSE` & `bepatient-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/PKG-INFO` & `bepatient-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bepatient
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library facilitating work with asynchronous APIs
 Author-email: Dawid Szaniawski <webluduspl@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Dawid Szaniawski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bepatient-0.8.1/README.md` & `bepatient-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/bepatient/__init__.py` & `bepatient-0.9.0/bepatient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     wait_for_value_in_request,
     wait_for_values_in_request,
 )
 from .waiter_src.checker import Checker
 from .waiter_src.checkers import CHECKERS
 from .waiter_src.comparators import COMPARATORS
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 __all__ = [
     "Checker",
     "CHECKERS",
     "COMPARATORS",
     "dict_differences",
     "RequestsWaiter",
     "to_curl",
```

### Comparing `bepatient-0.8.1/bepatient/api.py` & `bepatient-0.9.0/bepatient/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     """Utility class for setting up and monitoring requests for expected values.
 
     Args:
         request (PreparedRequest | Request | Response): request or response to monitor.
         status_code (int, optional): The expected HTTP status code. Defaults to 200.
         session (Session | None, optional): The requests session to use for sending
             requests. Defaults to None.
-        timeout (int | None, optional): request timeout in seconds.
+        timeout (int | tuple[int, int] | None, optional): request timeout in seconds.
+            Default value is 15 for connect and 30 for read (15, 30). If user provide
+            one value, it will be applied to both - connect and read timeouts.
 
     Example:
         To wait for a JSON response where the "status" field equals 200 using a
             RequestsWaiter:
         ```
             waiter = RequestsWaiter(request=requests, status_code=200, session=session)
             response = waiter.add_checker(
@@ -34,15 +36,15 @@
         ```"""
 
     def __init__(
         self,
         request: PreparedRequest | Request | Response,
         status_code: int = 200,
         session: Session | None = None,
-        timeout: int = 5,
+        timeout: int | tuple[int, int] | None = None,
     ):
         self.executor = RequestsExecutor(
             req_or_res=request,
             expected_status_code=status_code,
             session=session,
             timeout=timeout,
         )
@@ -50,36 +52,40 @@
     def add_checker(
         self,
         expected_value: Any,
         comparer: COMPARATORS,
         checker: CHECKERS = "json_checker",
         dict_path: str | None = None,
         search_query: str | None = None,
+        ignore_case: bool = False,
     ):
         """Add a response checker to the waiter.
 
         Args:
             expected_value (Any): The value to be compared against the response data.
             comparer (COMPARATORS): The comparer function or operator used for
                 value comparison.
             checker (CHECKERS, optional): The type of checker to use. Defaults to
                 "json_checker".
             dict_path (str | None, optional): The dot-separated path to the value in the
                 response data. Defaults to None.
             search_query (str | None, optional): A search query to use to find the value
                 in the response data. Defaults to None.
+            ignore_case (bool, optional): If set, upper/lower-case keys in dict_path
+                are treated the same. Defaults to False.
 
         Returns:
             self: updated RequestsWaiter instance."""
         self.executor.add_checker(
             RESPONSE_CHECKERS[checker](  # type: ignore
                 comparer=COMP_DICT[comparer],
                 expected_value=expected_value,
                 dict_path=dict_path,
                 search_query=search_query,
+                ignore_case=ignore_case,
             )
         )
         return self
 
     def add_custom_checker(self, checker: Checker):
         """Add a custom response checker to the waiter.
         This method allows users to add their own custom response checker by providing
@@ -131,14 +137,15 @@
     expected_value: Any = None,
     checker: CHECKERS = "json_checker",
     session: Session | None = None,
     dict_path: str | None = None,
     search_query: str | None = None,
     retries: int = 60,
     delay: int = 1,
+    req_timeout: int | tuple[int, int] | None = None,
 ) -> Response:
     """Wait for a specified value in a response.
 
     Args:
         request (PreparedRequest | Request | Response): The request or response to
             monitor for the expected value.
         status_code (int, optional): The expected HTTP status code. Defaults to 200.
@@ -151,14 +158,17 @@
             requests. Defaults to None.
         dict_path (str | None, optional): The dot-separated path to the value in the
             response data. Defaults to None.
         search_query (str | None, optional): A search query to use to find the value in
             the response data. Defaults to None.
         retries (int, optional): The number of retries to perform. Defaults to 60.
         delay (int, optional): The delay between retries in seconds. Defaults to 1.
+        req_timeout (int | tuple[int, int] | None, optional): request timeout in
+            seconds. Default value is 15 for connect and 30 for read (15, 30). If user
+            provide one value, it will be applied to both - connect and read timeouts.
 
     Returns:
         Response: the final response containing the expected value.
 
     Raises:
         WaiterConditionWasNotMet: if the condition is not met within the specified
             number of attempts.
@@ -173,15 +183,17 @@
                 comparer="have_len_greater",
                 expected_value=0,
                 checker="json_checker",
                 session=session,
                 dict_path="data",
             )
         ```"""
-    waiter = RequestsWaiter(request=request, status_code=status_code, session=session)
+    waiter = RequestsWaiter(
+        request=request, status_code=status_code, session=session, timeout=req_timeout
+    )
 
     if comparer:
         waiter.add_checker(
             comparer=comparer,
             checker=checker,
             expected_value=expected_value,
             dict_path=dict_path,
@@ -194,14 +206,15 @@
 def wait_for_values_in_request(
     request: PreparedRequest | Request | Response,
     checkers: list[dict[str, Any]],
     status_code: int = 200,
     session: Session | None = None,
     retries: int = 60,
     delay: int = 1,
+    req_timeout: int | tuple[int, int] | None = None,
 ) -> Response:
     """Wait for multiple specified values in a response using different checkers.
 
     Args:
         request (PreparedRequest | Request | Response): The request or response to
             monitor for the expected values.
         checkers (list[dict[str, Any]]): A list of dictionaries, where each dictionary
@@ -212,19 +225,24 @@
                     comparison.
                - expected_value (Any): the value to be compared against the response
                     data.
                - dict_path (str | None, optional): The dot-separated path to the value
                     in the response data. Defaults to None.
                - search_query (str | None, optional): A search query to use to find the
                     value in the response data. Defaults to None.
+               - ignore_case (bool, optional): If set, upper/lower-case keys in
+                    dict_path are treated the same. Defaults to False.
         status_code (int, optional): The expected HTTP status code. Defaults to 200.
         session (Session | None, optional): The requests session to use for sending
                requests. Defaults to None.
         retries (int, optional): The number of retries to perform. Defaults to 60.
         delay (int, optional): The delay between retries in seconds. Defaults to 1.
+        req_timeout (int | tuple[int, int] | None, optional): request timeout in
+            seconds. Default value is 15 for connect and 30 for read (15, 30). If user
+            provide one value, it will be applied to both - connect and read timeouts.
 
     Returns:
         Response: the final response containing the expected values.
 
     Raises:
         WaiterConditionWasNotMet: if the condition is not met within the specified
             number of attempts.
@@ -251,15 +269,17 @@
                request=request,
                checkers=checkers,
                status_code=200,
                session=session,
                retries=5
            )
         ```"""
-    waiter = RequestsWaiter(request=request, status_code=status_code, session=session)
+    waiter = RequestsWaiter(
+        request=request, status_code=status_code, session=session, timeout=req_timeout
+    )
 
     for checker_dict in checkers:
         waiter.add_checker(**checker_dict)
 
     return waiter.run(retries=retries, delay=delay).get_result()
```

### Comparing `bepatient-0.8.1/bepatient/curler.py` & `bepatient-0.9.0/bepatient/curler.py`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/bepatient/waiter_src/checker.py` & `bepatient-0.9.0/bepatient/waiter_src/checker.py`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/bepatient/waiter_src/checkers/response_checkers.py` & `bepatient-0.9.0/bepatient/waiter_src/checkers/response_checkers.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         expected_value (Any): The expected value to compare against.
         dict_path (str, optional): dot-separated path to the value in the response data.
             Defaults to None.
         search_query (str, optional): A search query to find the value in the response
             data. Defaults to None.
         dictor_fallback (str, optional): A default value to return if the value at the
             specified path is not found using `dictor`. Defaults to None.
+        ignore_case (bool, optional): If set, upper/lower-case keys in dict_path are
+            treated the same. Defaults to False.
 
     Example:
         To check if a specific field "status" in a JSON response equals 200:
 
         ```
             checker = JsonChecker(lambda a, b: a == b, 200, dict_path="status")
             assert checker.check(response) is True
@@ -54,19 +56,21 @@
     def __init__(
         self,
         comparer: Callable[[Any, Any], bool],
         expected_value: Any,
         dict_path: str | None = None,
         search_query: str | None = None,
         dictor_fallback: str | None = None,
+        ignore_case: bool = False,
     ):
         super().__init__(comparer, expected_value)
         self.path = dict_path
         self.search_query = search_query
         self.dictor_fallback = dictor_fallback
+        self.ignore_case = ignore_case
 
     @staticmethod
     def parse_response(
         data: Response, run_uuid: str | None = None
     ) -> dict[str, Any] | list[Any]:
         """Parse the response content as JSON for comparison.
 
@@ -90,14 +94,15 @@
             Any: The prepared data for comparison."""
         try:
             dictor_data = dictor(
                 data=self.parse_response(data, run_uuid),
                 path=self.path,
                 search=self.search_query,
                 default=self.dictor_fallback,
+                ignorecase=self.ignore_case,
             )
             log.info(
                 "Check uuid: %s | Dictor path: %s"
                 " | Dictor search: %s | Dictor data: %s",
                 run_uuid,
                 self.path,
                 self.search_query,
```

### Comparing `bepatient-0.8.1/bepatient/waiter_src/comparators.py` & `bepatient-0.9.0/bepatient/waiter_src/comparators.py`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/bepatient/waiter_src/executor.py` & `bepatient-0.9.0/bepatient/waiter_src/executor.py`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/bepatient/waiter_src/executors/requests_executor.py` & `bepatient-0.9.0/bepatient/waiter_src/executors/requests_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,27 +13,34 @@
 
 class RequestsExecutor(Executor):
     """An executor that sends a request and waits for a certain condition to be met.
     Args:
         req_or_res (PreparedRequest | Request | Response): request to send.
         expected_status_code (int): expected HTTP status code of the response
         session (Session | None, optional): requests session to use.
-        timeout (int | None, optional): request timeout in seconds."""
+        timeout (int | tuple[int, int] | None, optional): request timeout in seconds.
+            Default value is 15 for connect and 30 for read (15, 30). If user provide
+            one value, it will be applied to both - connect and read timeouts."""
 
     def __init__(
         self,
         req_or_res: PreparedRequest | Request | Response,
         expected_status_code: int,
         session: Session | None = None,
-        timeout: int = 5,
+        timeout: int | tuple[int, int] | None = None,
     ):
         super().__init__()
-        self.timeout = timeout
+
         self._status_code_checker = StatusCodeChecker(is_equal, expected_status_code)
 
+        if timeout:
+            self.timeout = timeout
+        else:
+            self.timeout = (15, 30)
+
         if session:
             self.session = session
         else:
             log.debug("Creating a new Session object")
             self.session = Session()
 
         if isinstance(req_or_res, Request):
```

### Comparing `bepatient-0.8.1/bepatient/waiter_src/waiter.py` & `bepatient-0.9.0/bepatient/waiter_src/waiter.py`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/bepatient.egg-info/PKG-INFO` & `bepatient-0.9.0/bepatient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bepatient
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library facilitating work with asynchronous APIs
 Author-email: Dawid Szaniawski <webluduspl@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Dawid Szaniawski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bepatient-0.8.1/bepatient.egg-info/SOURCES.txt` & `bepatient-0.9.0/bepatient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/pyproject.toml` & `bepatient-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/setup.cfg` & `bepatient-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/tests/test_api.py` & `bepatient-0.9.0/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,19 +92,19 @@
                 "bepatient.waiter_src.waiter",
                 20,
                 "Checking whether the condition has been met. The 1 approach",
             ),
             (
                 "bepatient.waiter_src.executors.requests_executor",
                 20,
-                "Sent: curl -X GET -H 'Content-Type: application/json'"
-                " -H 'Accept-Language: en-US,en;' -H 'Host: webludus.pl'"
-                " -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; rv:120.0)"
-                " Gecko/20100101' -H 'task: test' -H 'Cookie: pytest=fixture;"
-                " user-token=abc-123' https://webludus.pl/",
+                "Sent: curl -X GET -H 'Content-Type: application/json' -H"
+                " 'Accept-Language: en-US,en;' -H 'Host: webludus.pl' -H 'User-Agent:"
+                " Mozilla/5.0 (Windows NT 10.0; rv:120.0) Gecko/20100101' -H 'task:"
+                " test' -H 'Cookie: pytest=fixture; user-token=abc-123'"
+                " https://webludus.pl/",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: 1 | Checker: StatusCodeChecker | Comparer: is_equal"
                 " | Expected_value: 200 | Data: 200",
             ),
@@ -128,19 +128,19 @@
                 "bepatient.waiter_src.waiter",
                 20,
                 "Checking whether the condition has been met. The 2 approach",
             ),
             (
                 "bepatient.waiter_src.executors.requests_executor",
                 20,
-                "Sent: curl -X GET -H 'Content-Type: application/json'"
-                " -H 'Accept-Language: en-US,en;' -H 'Host: webludus.pl'"
-                " -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; rv:120.0)"
-                " Gecko/20100101' -H 'task: test' -H 'Cookie: pytest=fixture;"
-                " user-token=abc-123' https://webludus.pl/",
+                "Sent: curl -X GET -H 'Content-Type: application/json' -H"
+                " 'Accept-Language: en-US,en;' -H 'Host: webludus.pl' -H 'User-Agent:"
+                " Mozilla/5.0 (Windows NT 10.0; rv:120.0) Gecko/20100101' -H 'task:"
+                " test' -H 'Cookie: pytest=fixture; user-token=abc-123'"
+                " https://webludus.pl/",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: 2 | Checker: StatusCodeChecker | Comparer: is_equal"
                 " | Expected_value: 200 | Data: 200",
             ),
@@ -155,101 +155,102 @@
                 "Check success! | uuid: 2 | Checker: StatusCodeChecker"
                 " | Comparer: is_equal | Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: 3 | Checker: JsonChecker | Comparer: is_equal"
-                " | Dictor_fallback: None | Expected_value: Jack | Path: name"
-                " | Search_query: None | Data: Jack",
+                " | Dictor_fallback: None | Expected_value: Jack | Ignore_case: False"
+                " | Path: name | Search_query: None | Data: Jack",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 10,
                 "Check uuid: 3 | Response content: b''",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 40,
-                "Check uuid: 3 | Expected: Jack"
-                " | Headers: {'Content-Type': 'text/plain'} | Content b''",
+                "Check uuid: 3 | Expected: Jack | Headers:"
+                " {'Content-Type': 'text/plain'} | Content b''",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: 3 | Condition not met | Checker: JsonChecker"
                 " | Comparer: is_equal | Dictor_fallback: None | Expected_value: Jack"
-                " | Path: name | Search_query: None | Data: Jack",
+                " | Ignore_case: False | Path: name | Search_query: None | Data: Jack",
             ),
             (
                 "bepatient.waiter_src.waiter",
                 20,
                 "The condition has not been met. Waiting time: 1",
             ),
             (
                 "bepatient.waiter_src.waiter",
                 20,
                 "Checking whether the condition has been met. The 3 approach",
             ),
             (
                 "bepatient.waiter_src.executors.requests_executor",
                 20,
-                "Sent: curl -X GET -H 'Content-Type: application/json'"
-                " -H 'Accept-Language: en-US,en;' -H 'Host: webludus.pl'"
-                " -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; rv:120.0)"
-                " Gecko/20100101' -H 'task: test' -H 'Cookie: pytest=fixture;"
-                " user-token=abc-123' https://webludus.pl/",
+                "Sent: curl -X GET -H 'Content-Type: application/json' -H"
+                " 'Accept-Language: en-US,en;' -H 'Host: webludus.pl' -H 'User-Agent:"
+                " Mozilla/5.0 (Windows NT 10.0; rv:120.0) Gecko/20100101' -H 'task:"
+                " test' -H 'Cookie: pytest=fixture; user-token=abc-123'"
+                " https://webludus.pl/",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: 4 | Checker: StatusCodeChecker | Comparer: is_equal"
                 " | Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
-                "Check uuid: 4 | Response status code: 200 | Response content:"
-                ' b\'{"list_of_dicts": [{"name": "John", "age": 30}, {"name": "Mike",'
+                "Check uuid: 4 | Response status code: 200 | Response content: "
+                'b\'{"list_of_dicts": [{"name": "John", "age": 30}, {"name": "Mike",'
                 ' "age": 15}], "ok": true, "some_number": 123, "list": ["1", "2", "3"],'
-                ' "none": null, "empty": "", "false": false, "name": "Jack"}\'',
+                ' "none": null, "empty": "", "false": false, "name": "Jack",'
+                ' "City": "Cracow"}\'',
             ),
             (
                 "bepatient.waiter_src.checker",
                 10,
                 "Check success! | uuid: 4 | Checker: StatusCodeChecker"
                 " | Comparer: is_equal | Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: 5 | Checker: JsonChecker | Comparer: is_equal"
-                " | Dictor_fallback: None | Expected_value: Jack | Path: name"
-                " | Search_query: None | Data: Jack",
+                " | Dictor_fallback: None | Expected_value: Jack | Ignore_case: False"
+                " | Path: name | Search_query: None | Data: Jack",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 10,
                 'Check uuid: 5 | Response content: b\'{"list_of_dicts": [{"name":'
                 ' "John", "age": 30}, {"name": "Mike", "age": 15}], "ok": true,'
                 ' "some_number": 123, "list": ["1", "2", "3"], "none": null, "empty":'
-                ' "", "false": false, "name": "Jack"}\'',
+                ' "", "false": false, "name": "Jack", "City": "Cracow"}\'',
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
                 "Check uuid: 5 | Dictor path: name | Dictor search: None"
                 " | Dictor data: Jack",
             ),
             (
                 "bepatient.waiter_src.checker",
                 10,
                 "Check success! | uuid: 5 | Checker: JsonChecker | Comparer: is_equal"
-                " | Dictor_fallback: None | Expected_value: Jack | Path: name"
-                " | Search_query: None | Data: Jack",
+                " | Dictor_fallback: None | Expected_value: Jack | Ignore_case: False"
+                " | Path: name | Search_query: None | Data: Jack",
             ),
             ("bepatient.waiter_src.waiter", 20, "Condition met!"),
         ]
 
         waiter = RequestsWaiter(request=request_object, session=session_object)
         waiter.add_checker(expected_value="Jack", comparer="is_equal", dict_path="name")
         res_json = waiter.run(retries=3).get_result().json()
@@ -296,24 +297,24 @@
                 20,
                 "Checking whether the condition has been met. The 1 approach",
             ),
             (
                 "bepatient.waiter_src.executors.requests_executor",
                 20,
                 "Sent: curl -X GET -H 'task: test' -H 'Cookie: user-token=abc-123;"
-                " pytest=fixture' -H 'Content-Type: application/json'"
-                " -H 'Accept-Language: en-US,en;' -H 'Host: webludus.pl'"
-                " -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; rv:120.0)"
-                " Gecko/20100101' https://webludus.pl/",
+                " pytest=fixture' -H 'Content-Type: application/json' -H"
+                " 'Accept-Language: en-US,en;' -H 'Host: webludus.pl' -H 'User-Agent:"
+                " Mozilla/5.0 (Windows NT 10.0; rv:120.0) Gecko/20100101'"
+                " https://webludus.pl/",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
-                "Check uuid: A | Checker: StatusCodeChecker | Comparer: is_equal"
-                " | Expected_value: 200 | Data: 200",
+                "Check uuid: A | Checker: StatusCodeChecker | Comparer: is_equal | "
+                "Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
                 "Check uuid: A | Response status code: 404 | Response content: b''",
             ),
             (
@@ -331,67 +332,69 @@
                 "bepatient.waiter_src.waiter",
                 20,
                 "Checking whether the condition has been met. The 2 approach",
             ),
             (
                 "bepatient.waiter_src.executors.requests_executor",
                 20,
-                "Sent: curl -X GET -H 'task: test' -H 'Cookie: user-token=abc-123;"
-                " pytest=fixture' -H 'Content-Type: application/json'"
-                " -H 'Accept-Language: en-US,en;' -H 'Host: webludus.pl'"
-                " -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; rv:120.0)"
-                " Gecko/20100101' https://webludus.pl/",
+                "Sent: curl -X GET -H 'task: test' -H 'Cookie: user-token=abc-123; "
+                "pytest=fixture' -H 'Content-Type: application/json' -H"
+                " 'Accept-Language: en-US,en;' -H 'Host: webludus.pl' -H 'User-Agent:"
+                " Mozilla/5.0 (Windows NT 10.0; rv:120.0) Gecko/20100101'"
+                " https://webludus.pl/",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
-                "Check uuid: B | Checker: StatusCodeChecker | Comparer: is_equal"
-                " | Expected_value: 200 | Data: 200",
+                "Check uuid: B | Checker: StatusCodeChecker | Comparer: is_equal | "
+                "Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
-                "Check uuid: B | Response status code: 200 | Response content:"
-                ' b\'{"list_of_dicts": [{"name": "John", "age": 30}, {"name": "Mike",'
+                "Check uuid: B | Response status code: 200 | Response content: "
+                'b\'{"list_of_dicts": [{"name": "John", "age": 30}, {"name": "Mike",'
                 ' "age": 15}], "ok": true, "some_number": 123, "list": ["1", "2", "3"],'
-                ' "none": null, "empty": "", "false": false, "name": "Jack"}\'',
+                ' "none": null, "empty": "", "false": false, "name": "Jack",'
+                ' "City": "Cracow"}\'',
             ),
             (
                 "bepatient.waiter_src.checker",
                 10,
                 "Check success! | uuid: B | Checker: StatusCodeChecker"
                 " | Comparer: is_equal | Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: C | Checker: HeadersChecker | Comparer: is_equal"
                 " | Dictor_fallback: None | Expected_value: gunicorn"
-                " | Path: X-Render-Origin_Server | Search_query: None | Data: gunicorn",
+                " | Ignore_case: False | Path: X-Render-Origin_Server"
+                " | Search_query: None | Data: gunicorn",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
-                "Check uuid: C | Response headers: {'Content-Language': 'en-US',"
-                " 'Content-Type': 'application/json', 'Server': 'WebLudus.pl',"
-                " 'X-Render-Origin_Server': 'gunicorn'}",
+                "Check uuid: C | Response headers: {'Content-Language': 'en-US', "
+                "'Content-Type': 'application/json', 'Server': 'WebLudus.pl', "
+                "'X-Render-Origin_Server': 'gunicorn'}",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
                 "Check uuid: C | Dictor path: X-Render-Origin_Server"
                 " | Dictor search: None | Dictor data: gunicorn",
             ),
             (
                 "bepatient.waiter_src.checker",
                 10,
                 "Check success! | uuid: C | Checker: HeadersChecker"
                 " | Comparer: is_equal | Dictor_fallback: None"
-                " | Expected_value: gunicorn | Path: X-Render-Origin_Server"
-                " | Search_query: None | Data: gunicorn",
+                " | Expected_value: gunicorn | Ignore_case: False"
+                " | Path: X-Render-Origin_Server | Search_query: None | Data: gunicorn",
             ),
             ("bepatient.waiter_src.waiter", 20, "Condition met!"),
         ]
 
         waiter = RequestsWaiter(request=example_response, session=session_object)
         waiter.add_checker(
             expected_value="gunicorn",
@@ -499,16 +502,17 @@
                 "Check success! | uuid: TEST1 | Checker: StatusCodeChecker"
                 " | Comparer: is_equal | Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: TEST2 | Checker: HeadersChecker | Comparer: is_equal"
-                " | Dictor_fallback: None | Expected_value: WebLudus.pl | Path: Server"
-                " | Search_query: None | Data: WebLudus.pl",
+                " | Dictor_fallback: None | Expected_value: WebLudus.pl"
+                " | Ignore_case: False | Path: Server | Search_query: None"
+                " | Data: WebLudus.pl",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
                 "Check uuid: TEST2 | Response headers: {}",
             ),
             (
@@ -518,59 +522,61 @@
                 " | Dictor data: None",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: TEST2 | Condition not met | Checker: HeadersChecker"
                 " | Comparer: is_equal | Dictor_fallback: None"
-                " | Expected_value: WebLudus.pl | Path: Server | Search_query: None"
-                " | Data: WebLudus.pl",
+                " | Expected_value: WebLudus.pl | Ignore_case: False | Path: Server"
+                " | Search_query: None | Data: WebLudus.pl",
             ),
             (
                 "bepatient.waiter_src.waiter",
                 20,
                 "The condition has not been met. Waiting time: 1",
             ),
             (
                 "bepatient.waiter_src.waiter",
                 20,
                 "Checking whether the condition has been met. The 2 approach",
             ),
             (
                 "bepatient.waiter_src.executors.requests_executor",
                 20,
-                "Sent: curl -X GET -H 'task: test' -H 'Cookie: user-token=abc-123'"
-                " https://webludus.pl/",
+                "Sent: curl -X GET -H 'task: test' -H 'Cookie: user-token=abc-123' "
+                "https://webludus.pl/",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: TEST3 | Checker: StatusCodeChecker | Comparer: is_equal"
                 " | Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
                 "Check uuid: TEST3 | Response status code: 200 | Response content:"
                 ' b\'{"list_of_dicts": [{"name": "John", "age": 30}, {"name": "Mike",'
                 ' "age": 15}], "ok": true, "some_number": 123, "list": ["1", "2", "3"],'
-                ' "none": null, "empty": "", "false": false, "name": "Jack"}\'',
+                ' "none": null, "empty": "", "false": false, "name": "Jack",'
+                ' "City": "Cracow"}\'',
             ),
             (
                 "bepatient.waiter_src.checker",
                 10,
-                "Check success! | uuid: TEST3 | Checker: StatusCodeChecker"
-                " | Comparer: is_equal | Expected_value: 200 | Data: 200",
+                "Check success! | uuid: TEST3 | Checker: StatusCodeChecker | Comparer: "
+                "is_equal | Expected_value: 200 | Data: 200",
             ),
             (
                 "bepatient.waiter_src.checker",
                 20,
                 "Check uuid: TEST4 | Checker: HeadersChecker | Comparer: is_equal"
-                " | Dictor_fallback: None | Expected_value: WebLudus.pl | Path: Server"
-                " | Search_query: None | Data: WebLudus.pl",
+                " | Dictor_fallback: None | Expected_value: WebLudus.pl"
+                " | Ignore_case: False | Path: Server | Search_query: None"
+                " | Data: WebLudus.pl",
             ),
             (
                 "bepatient.waiter_src.checkers.response_checkers",
                 20,
                 "Check uuid: TEST4 | Response headers: {'Content-Language': 'en-US',"
                 " 'Content-Type': 'application/json', 'Server': 'WebLudus.pl',"
                 " 'X-Render-Origin_Server': 'gunicorn'}",
@@ -582,16 +588,16 @@
                 " | Dictor data: WebLudus.pl",
             ),
             (
                 "bepatient.waiter_src.checker",
                 10,
                 "Check success! | uuid: TEST4 | Checker: HeadersChecker"
                 " | Comparer: is_equal | Dictor_fallback: None"
-                " | Expected_value: WebLudus.pl | Path: Server | Search_query: None"
-                " | Data: WebLudus.pl",
+                " | Expected_value: WebLudus.pl | Ignore_case: False | Path: Server"
+                " | Search_query: None | Data: WebLudus.pl",
             ),
             ("bepatient.waiter_src.waiter", 20, "Condition met!"),
         ]
 
         waiter = RequestsWaiter(request=prepared_request)
         waiter.add_checker(
             expected_value="WebLudus.pl",
```

### Comparing `bepatient-0.8.1/tests/test_curler.py` & `bepatient-0.9.0/tests/test_curler.py`

 * *Files identical despite different names*

### Comparing `bepatient-0.8.1/tests/test_e2e.py` & `bepatient-0.9.0/tests/test_e2e.py`

 * *Files identical despite different names*

