# Comparing `tmp/glibs-www-1.0.0.tar.gz` & `tmp/glibs-www-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glibs-www-1.0.0.tar", last modified: Wed Jan 19 04:48:52 2022, max compression
+gzip compressed data, was "dist/glibs-www-2.0.2.tar", last modified: Mon Apr  1 18:33:49 2024, max compression
```

## Comparing `glibs-www-1.0.0.tar` & `glibs-www-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 lucas      (501) staff       (20)        0 2022-01-19 04:48:52.964690 glibs-www-1.0.0/
--rw-r--r--   0 lucas      (501) staff       (20)      221 2022-01-19 04:48:52.964749 glibs-www-1.0.0/PKG-INFO
--rw-r--r--   0 lucas      (501) staff       (20)       11 2022-01-18 13:07:36.000000 glibs-www-1.0.0/README.md
-drwxr-xr-x   0 lucas      (501) staff       (20)        0 2022-01-19 04:48:52.963252 glibs-www-1.0.0/glibs/
--rw-r--r--   0 lucas      (501) staff       (20)       56 2022-01-18 13:07:36.000000 glibs-www-1.0.0/glibs/__init__.py
-drwxr-xr-x   0 lucas      (501) staff       (20)        0 2022-01-19 04:48:52.963971 glibs-www-1.0.0/glibs/www/
--rw-r--r--   0 lucas      (501) staff       (20)        0 2022-01-18 13:07:36.000000 glibs-www-1.0.0/glibs/www/__init__.py
--rw-r--r--   0 lucas      (501) staff       (20)     1850 2022-01-18 13:07:36.000000 glibs-www-1.0.0/glibs/www/log_extra_info_on_4xx5xx_errors.py
--rw-r--r--   0 lucas      (501) staff       (20)     1559 2022-01-18 15:46:49.000000 glibs-www-1.0.0/glibs/www/request_logger.py
--rw-r--r--   0 lucas      (501) staff       (20)     2042 2022-01-18 13:07:36.000000 glibs-www-1.0.0/glibs/www/timeout.py
-drwxr-xr-x   0 lucas      (501) staff       (20)        0 2022-01-19 04:48:52.964597 glibs-www-1.0.0/glibs_www.egg-info/
--rw-r--r--   0 lucas      (501) staff       (20)      221 2022-01-19 04:48:52.000000 glibs-www-1.0.0/glibs_www.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (501) staff       (20)      351 2022-01-19 04:48:52.000000 glibs-www-1.0.0/glibs_www.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (501) staff       (20)        1 2022-01-19 04:48:52.000000 glibs-www-1.0.0/glibs_www.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (501) staff       (20)        6 2022-01-19 04:48:52.000000 glibs-www-1.0.0/glibs_www.egg-info/namespace_packages.txt
--rw-r--r--   0 lucas      (501) staff       (20)        6 2022-01-19 04:48:52.000000 glibs-www-1.0.0/glibs_www.egg-info/top_level.txt
--rw-r--r--   0 lucas      (501) staff       (20)       94 2022-01-18 13:07:36.000000 glibs-www-1.0.0/pyproject.toml
--rw-r--r--   0 lucas      (501) staff       (20)      340 2022-01-19 04:48:52.964982 glibs-www-1.0.0/setup.cfg
--rw-r--r--   0 lucas      (501) staff       (20)       84 2022-01-18 13:07:36.000000 glibs-www-1.0.0/setup.py
+drwxr-xr-x   0 Geekie     (502) staff       (20)        0 2024-04-01 18:33:49.858070 glibs-www-2.0.2/
+-rw-r--r--   0 Geekie     (502) staff       (20)      139 2024-04-01 18:33:49.857842 glibs-www-2.0.2/PKG-INFO
+-rw-r--r--   0 Geekie     (502) staff       (20)       11 2024-03-28 23:22:27.000000 glibs-www-2.0.2/README.md
+drwxr-xr-x   0 Geekie     (502) staff       (20)        0 2024-04-01 18:33:49.847128 glibs-www-2.0.2/glibs/
+-rw-r--r--   0 Geekie     (502) staff       (20)       56 2024-03-28 23:22:27.000000 glibs-www-2.0.2/glibs/__init__.py
+drwxr-xr-x   0 Geekie     (502) staff       (20)        0 2024-04-01 18:33:49.849863 glibs-www-2.0.2/glibs/www/
+-rw-r--r--   0 Geekie     (502) staff       (20)        0 2024-03-28 23:22:27.000000 glibs-www-2.0.2/glibs/www/__init__.py
+-rw-r--r--   0 Geekie     (502) staff       (20)     1850 2024-03-28 23:22:27.000000 glibs-www-2.0.2/glibs/www/log_extra_info_on_4xx5xx_errors.py
+-rw-r--r--   0 Geekie     (502) staff       (20)     1559 2024-03-28 23:22:27.000000 glibs-www-2.0.2/glibs/www/request_logger.py
+-rw-r--r--   0 Geekie     (502) staff       (20)     2442 2024-03-28 23:22:27.000000 glibs-www-2.0.2/glibs/www/timeout.py
+drwxr-xr-x   0 Geekie     (502) staff       (20)        0 2024-04-01 18:33:49.857001 glibs-www-2.0.2/glibs_www.egg-info/
+-rw-r--r--   0 Geekie     (502) staff       (20)      139 2024-04-01 18:33:49.000000 glibs-www-2.0.2/glibs_www.egg-info/PKG-INFO
+-rw-r--r--   0 Geekie     (502) staff       (20)      448 2024-04-01 18:33:49.000000 glibs-www-2.0.2/glibs_www.egg-info/SOURCES.txt
+-rw-r--r--   0 Geekie     (502) staff       (20)        1 2024-04-01 18:33:49.000000 glibs-www-2.0.2/glibs_www.egg-info/dependency_links.txt
+-rw-r--r--   0 Geekie     (502) staff       (20)        6 2024-04-01 18:33:49.000000 glibs-www-2.0.2/glibs_www.egg-info/namespace_packages.txt
+-rw-r--r--   0 Geekie     (502) staff       (20)        6 2024-04-01 18:33:49.000000 glibs-www-2.0.2/glibs_www.egg-info/top_level.txt
+-rw-r--r--   0 Geekie     (502) staff       (20)       94 2024-03-28 23:22:27.000000 glibs-www-2.0.2/pyproject.toml
+-rw-r--r--   0 Geekie     (502) staff       (20)      339 2024-04-01 18:33:49.859082 glibs-www-2.0.2/setup.cfg
+-rw-r--r--   0 Geekie     (502) staff       (20)      185 2024-04-01 12:58:50.000000 glibs-www-2.0.2/setup.py
+drwxr-xr-x   0 Geekie     (502) staff       (20)        0 2024-04-01 18:33:49.856135 glibs-www-2.0.2/tests/
+-rw-r--r--   0 Geekie     (502) staff       (20)     4874 2024-03-28 23:22:27.000000 glibs-www-2.0.2/tests/test_log_extra_info_on_4xx5xx_errors.py
+-rw-r--r--   0 Geekie     (502) staff       (20)     2975 2024-03-28 23:22:27.000000 glibs-www-2.0.2/tests/test_request_logger.py
+-rw-r--r--   0 Geekie     (502) staff       (20)     3272 2024-03-28 23:22:27.000000 glibs-www-2.0.2/tests/test_timeout.py
```

### Comparing `glibs-www-1.0.0/glibs/www/log_extra_info_on_4xx5xx_errors.py` & `glibs-www-2.0.2/glibs/www/log_extra_info_on_4xx5xx_errors.py`

 * *Files identical despite different names*

### Comparing `glibs-www-1.0.0/glibs/www/request_logger.py` & `glibs-www-2.0.2/glibs/www/request_logger.py`

 * *Files identical despite different names*

### Comparing `glibs-www-1.0.0/glibs/www/timeout.py` & `glibs-www-2.0.2/glibs/www/timeout.py`

 * *Files 27% similar despite different names*

```diff
@@ -57,22 +57,28 @@
 
 
 def bind_pyramid(config):
     config.add_tween("glibs.www.timeout.pyramid_tween")
 
 
 def pyramid_tween(handler, registry):
-    timeout_seconds = int(registry.settings.get("gevent_timeout", "30"))
+    custom_timeout_by_endpoint = registry.settings.get("custom_timeout_by_endpoint", {})
+    default_timeout_in_seconds = int(registry.settings.get("gevent_timeout", "30"))
 
     def request_timeout(request):
-        timeout = _timeout(timeout_seconds)
+        if request.path in custom_timeout_by_endpoint.keys():
+            timeout = _timeout(int(custom_timeout_by_endpoint[request.path]))
+            max_time_to_wait = custom_timeout_by_endpoint[request.path]
+        else:
+            timeout = _timeout(default_timeout_in_seconds)
+            max_time_to_wait = default_timeout_in_seconds
         timeout.start()
         start_time = time.time()
         try:
             result = handler(request)
-            if time.time() - start_time > timeout_seconds:
+            if time.time() - start_time > max_time_to_wait:
                 raise DeadlineExceededError()
             return result
         finally:
             timeout.close()
 
     return request_timeout
```

