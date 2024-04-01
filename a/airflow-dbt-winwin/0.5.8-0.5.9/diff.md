# Comparing `tmp/airflow-dbt-winwin-0.5.8.tar.gz` & `tmp/airflow-dbt-winwin-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-dbt-winwin-0.5.8.tar", last modified: Wed Mar 27 02:56:32 2024, max compression
+gzip compressed data, was "airflow-dbt-winwin-0.5.9.tar", last modified: Fri Mar 29 07:59:26 2024, max compression
```

## Comparing `airflow-dbt-winwin-0.5.8.tar` & `airflow-dbt-winwin-0.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-27 02:56:32.787330 airflow-dbt-winwin-0.5.8/
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1067 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.8/LICENSE.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)       25 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.8/MANIFEST.in
--rw-r--r--   0 leezhongshan   (501) staff       (20)     6923 2024-03-27 02:56:32.787088 airflow-dbt-winwin-0.5.8/PKG-INFO
--rw-r--r--   0 leezhongshan   (501) staff       (20)     6333 2024-03-05 06:30:04.000000 airflow-dbt-winwin-0.5.8/README.md
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-27 02:56:32.785010 airflow-dbt-winwin-0.5.8/airflow_dbt/
--rw-r--r--   0 leezhongshan   (501) staff       (20)      193 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt/__init__.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)       65 2024-03-27 02:55:35.000000 airflow-dbt-winwin-0.5.8/airflow_dbt/__version__.py
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-27 02:56:32.785378 airflow-dbt-winwin-0.5.8/airflow_dbt/hooks/
--rw-r--r--   0 leezhongshan   (501) staff       (20)       33 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt/hooks/__init__.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     7680 2024-03-27 02:20:45.000000 airflow-dbt-winwin-0.5.8/airflow_dbt/hooks/dbt_hook.py
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-27 02:56:32.785911 airflow-dbt-winwin-0.5.8/airflow_dbt/operators/
--rw-r--r--   0 leezhongshan   (501) staff       (20)      166 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt/operators/__init__.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     5292 2024-03-26 10:02:13.000000 airflow-dbt-winwin-0.5.8/airflow_dbt/operators/dbt_operator.py
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-27 02:56:32.786676 airflow-dbt-winwin-0.5.8/airflow_dbt_winwin.egg-info/
--rw-r--r--   0 leezhongshan   (501) staff       (20)     6923 2024-03-27 02:56:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt_winwin.egg-info/PKG-INFO
--rw-r--r--   0 leezhongshan   (501) staff       (20)      434 2024-03-27 02:56:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt_winwin.egg-info/SOURCES.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)        1 2024-03-27 02:56:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt_winwin.egg-info/dependency_links.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)       23 2024-03-27 02:56:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt_winwin.egg-info/requires.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)       12 2024-03-27 02:56:32.000000 airflow-dbt-winwin-0.5.8/airflow_dbt_winwin.egg-info/top_level.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)       38 2024-03-27 02:56:32.787372 airflow-dbt-winwin-0.5.8/setup.cfg
--rw-r--r--   0 leezhongshan   (501) staff       (20)     2225 2023-12-27 08:46:15.000000 airflow-dbt-winwin-0.5.8/setup.py
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-29 07:59:26.658594 airflow-dbt-winwin-0.5.9/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1067 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.9/LICENSE.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       25 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.9/MANIFEST.in
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     6885 2024-03-29 07:59:26.658459 airflow-dbt-winwin-0.5.9/PKG-INFO
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     6333 2024-03-05 06:30:04.000000 airflow-dbt-winwin-0.5.9/README.md
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-29 07:59:26.656769 airflow-dbt-winwin-0.5.9/airflow_dbt/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      193 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.9/airflow_dbt/__init__.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       63 2024-03-29 07:59:10.000000 airflow-dbt-winwin-0.5.9/airflow_dbt/__version__.py
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-29 07:59:26.657126 airflow-dbt-winwin-0.5.9/airflow_dbt/hooks/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       33 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.9/airflow_dbt/hooks/__init__.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     7820 2024-03-29 07:57:41.000000 airflow-dbt-winwin-0.5.9/airflow_dbt/hooks/dbt_hook.py
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-29 07:59:26.657505 airflow-dbt-winwin-0.5.9/airflow_dbt/operators/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      166 2023-12-27 08:21:32.000000 airflow-dbt-winwin-0.5.9/airflow_dbt/operators/__init__.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     5356 2024-03-29 07:55:46.000000 airflow-dbt-winwin-0.5.9/airflow_dbt/operators/dbt_operator.py
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-03-29 07:59:26.658238 airflow-dbt-winwin-0.5.9/airflow_dbt_winwin.egg-info/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     6885 2024-03-29 07:59:26.000000 airflow-dbt-winwin-0.5.9/airflow_dbt_winwin.egg-info/PKG-INFO
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      434 2024-03-29 07:59:26.000000 airflow-dbt-winwin-0.5.9/airflow_dbt_winwin.egg-info/SOURCES.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)        1 2024-03-29 07:59:26.000000 airflow-dbt-winwin-0.5.9/airflow_dbt_winwin.egg-info/dependency_links.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       23 2024-03-29 07:59:26.000000 airflow-dbt-winwin-0.5.9/airflow_dbt_winwin.egg-info/requires.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       12 2024-03-29 07:59:26.000000 airflow-dbt-winwin-0.5.9/airflow_dbt_winwin.egg-info/top_level.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       38 2024-03-29 07:59:26.658637 airflow-dbt-winwin-0.5.9/setup.cfg
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     2225 2023-12-27 08:46:15.000000 airflow-dbt-winwin-0.5.9/setup.py
```

### Comparing `airflow-dbt-winwin-0.5.8/LICENSE.txt` & `airflow-dbt-winwin-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow-dbt-winwin-0.5.8/PKG-INFO` & `airflow-dbt-winwin-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: airflow-dbt-winwin
-Version: 0.5.8
+Version: 0.5.9
 Summary: Apache Airflow integration for dbt
 Home-page: https://github.com/gocardless/airflow-dbt
 Author: GoCardless
 Author-email: engineering@gocardless.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: apache-airflow>=1.10.3
 
 # airflow-dbt
 
 This is a collection of [Airflow](https://airflow.apache.org/) operators to provide easy integration with [dbt](https://www.getdbt.com).
 
 ```py
 from airflow import DAG
```

### Comparing `airflow-dbt-winwin-0.5.8/README.md` & `airflow-dbt-winwin-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `airflow-dbt-winwin-0.5.8/airflow_dbt/hooks/dbt_hook.py` & `airflow-dbt-winwin-0.5.9/airflow_dbt/hooks/dbt_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
                  select=None,
                  selector=None,
                  debug=False,
                  dbt_bin='dbt',
                  output_encoding='utf-8',
                  verbose=True,
                  warn_error=False,
-                 append_env = False
+                 append_env = False,
+                 threads = None
                  ):
         super().__init__()
 
 
         self.context = context
         self.env = env or {} 
         self.profiles_dir = profiles_dir
@@ -83,14 +84,15 @@
         self.selector = selector
         self.debug = debug  
         self.dbt_bin = dbt_bin
         self.verbose = verbose
         self.warn_error = warn_error
         self.output_encoding = output_encoding
         self.append_env = append_env
+        self.threads = threads
         
 
     def get_env(self, context, env ):
         """Build the set of environment variables to be exposed for the bash command."""
         system_env = os.environ.copy()
          
         if env is None:
@@ -154,24 +156,29 @@
             dbt_cmd.extend(['--exclude', self.exclude])
 
         if self.select is not None:
             dbt_cmd.extend(['--select', self.select])
 
         if self.selector is not None:
             dbt_cmd.extend(['--selector', self.selector])
-        
+
+        if self.threads:
+            dbt_cmd.extend(['--threads', self.threads])
+
         if self.debug:
             dbt_cmd.extend(['--debug'])
 
         if self.full_refresh:
             dbt_cmd.extend(['--full-refresh'])
 
+
         if self.warn_error:
             dbt_cmd.insert(1, '--warn-error')
 
+
         if self.verbose:
             self.log.info(" ".join(dbt_cmd))
         
         sub_env = self.get_env(self.context, self.env)
         self.log.info(f"subprocess env: {sub_env}")
         sp = subprocess.Popen(
             dbt_cmd,
```

### Comparing `airflow-dbt-winwin-0.5.8/airflow_dbt/operators/dbt_operator.py` & `airflow-dbt-winwin-0.5.9/airflow_dbt/operators/dbt_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
                  debug=False,
                  dbt_bin='dbt',
                  verbose=True,
                  warn_error=False,
                  full_refresh=False,
                  data=False,
                  schema=False,
+                 threads = None,
                  *args,
                  **kwargs):
         super().__init__(*args, **kwargs)
 
         self.env = env or {}
         self.profiles_dir = profiles_dir
         self.target = target
@@ -92,14 +93,15 @@
         self.select = select
         self.selector = selector
         self.debug = debug 
         self.dbt_bin = dbt_bin
         self.verbose = verbose
         self.warn_error = warn_error
         self.hook = None
+        self.threads = threads
 
     def create_hook(self, context):
         if self.hook  is None:
             self.hook = DbtCliHook(
                 context = context,
                 env=self.env,
                 profiles_dir=self.profiles_dir,
```

### Comparing `airflow-dbt-winwin-0.5.8/airflow_dbt_winwin.egg-info/PKG-INFO` & `airflow-dbt-winwin-0.5.9/airflow_dbt_winwin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: airflow-dbt-winwin
-Version: 0.5.8
+Version: 0.5.9
 Summary: Apache Airflow integration for dbt
 Home-page: https://github.com/gocardless/airflow-dbt
 Author: GoCardless
 Author-email: engineering@gocardless.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: apache-airflow>=1.10.3
 
 # airflow-dbt
 
 This is a collection of [Airflow](https://airflow.apache.org/) operators to provide easy integration with [dbt](https://www.getdbt.com).
 
 ```py
 from airflow import DAG
```

### Comparing `airflow-dbt-winwin-0.5.8/setup.py` & `airflow-dbt-winwin-0.5.9/setup.py`

 * *Files identical despite different names*

