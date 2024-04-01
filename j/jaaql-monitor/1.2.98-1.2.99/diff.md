# Comparing `tmp/jaaql-monitor-1.2.98.tar.gz` & `tmp/jaaql-monitor-1.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.98.tar", last modified: Fri Oct  6 08:08:26 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.99.tar", last modified: Wed Oct 18 11:20:20 2023, max compression
```

## Comparing `jaaql-monitor-1.2.98.tar` & `jaaql-monitor-1.2.99.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-10-06 08:08:26.515281 jaaql-monitor-1.2.98/
--rw-rw-rw-   0        0        0    18124 2023-10-05 22:57:32.000000 jaaql-monitor-1.2.98/LICENSE.txt
--rw-rw-rw-   0        0        0     1476 2023-10-06 08:08:26.515281 jaaql-monitor-1.2.98/PKG-INFO
--rw-rw-rw-   0        0        0     1064 2023-10-05 22:58:34.000000 jaaql-monitor-1.2.98/README.md
-drwxrwxrwx   0        0        0        0 2023-10-06 08:08:26.515281 jaaql-monitor-1.2.98/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1476 2023-10-06 08:08:26.000000 jaaql-monitor-1.2.98/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-10-06 08:08:26.000000 jaaql-monitor-1.2.98/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-06 08:08:26.000000 jaaql-monitor-1.2.98/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-10-06 08:08:26.000000 jaaql-monitor-1.2.98/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-06 08:08:26.000000 jaaql-monitor-1.2.98/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-06 08:08:26.515281 jaaql-monitor-1.2.98/monitor/
--rw-rw-rw-   0        0        0        0 2023-10-05 22:57:32.000000 jaaql-monitor-1.2.98/monitor/__init__.py
--rw-rw-rw-   0        0        0    33230 2023-10-06 08:06:27.000000 jaaql-monitor-1.2.98/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-10-06 08:08:19.000000 jaaql-monitor-1.2.98/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-10-06 08:08:26.515281 jaaql-monitor-1.2.98/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-10-05 22:57:32.000000 jaaql-monitor-1.2.98/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-18 11:20:20.540320 jaaql-monitor-1.2.99/
+-rw-rw-rw-   0        0        0    18124 2023-10-05 22:57:32.000000 jaaql-monitor-1.2.99/LICENSE.txt
+-rw-rw-rw-   0        0        0     1476 2023-10-18 11:20:20.540320 jaaql-monitor-1.2.99/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2023-10-05 22:58:34.000000 jaaql-monitor-1.2.99/README.md
+drwxrwxrwx   0        0        0        0 2023-10-18 11:20:20.540320 jaaql-monitor-1.2.99/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1476 2023-10-18 11:20:20.000000 jaaql-monitor-1.2.99/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-10-18 11:20:20.000000 jaaql-monitor-1.2.99/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-18 11:20:20.000000 jaaql-monitor-1.2.99/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-10-18 11:20:20.000000 jaaql-monitor-1.2.99/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-10-18 11:20:20.000000 jaaql-monitor-1.2.99/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-18 11:20:20.540320 jaaql-monitor-1.2.99/monitor/
+-rw-rw-rw-   0        0        0        0 2023-10-05 22:57:32.000000 jaaql-monitor-1.2.99/monitor/__init__.py
+-rw-rw-rw-   0        0        0    33540 2023-10-18 11:20:00.000000 jaaql-monitor-1.2.99/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-10-18 11:20:12.000000 jaaql-monitor-1.2.99/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-10-18 11:20:20.540320 jaaql-monitor-1.2.99/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-10-05 22:57:32.000000 jaaql-monitor-1.2.99/setup.py
```

### Comparing `jaaql-monitor-1.2.98/LICENSE.txt` & `jaaql-monitor-1.2.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.98/PKG-INFO` & `jaaql-monitor-1.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.98
+Version: 1.2.99
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.98/README.md` & `jaaql-monitor-1.2.99/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.98/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.99/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.98
+Version: 1.2.99
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.98/monitor/main.py` & `jaaql-monitor-1.2.99/monitor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,22 @@
             self._fetch_oauth_token_for_current_connection()
             start_time = datetime.now()
             res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
 
         self.log("Request took " + str(self.time_delta_ms(start_time, datetime.now())) + "ms")
 
         if res.status_code == 200 and format_as_query_output:
-            format_query_output(self, res.json())
+            was_explain = False
+            if "query" in send_json:
+                was_explain = len([line.strip().startswith("EXPLAIN ANALYZE") for line in split_by_lines(send_json["query"])]) != 0
+
+            if was_explain:
+                self.log(res.json()["rows"][0][0])
+            else:
+                format_query_output(self, res.json())
         elif res.status_code == 200:
             print(json.dumps(res.json(), indent=4))
         else:
             if handle_error:
                 if endpoint == ENDPOINT__submit:
                     submit_error(self, res.text)
                 else:
```

### Comparing `jaaql-monitor-1.2.98/setup.py` & `jaaql-monitor-1.2.99/setup.py`

 * *Files identical despite different names*

