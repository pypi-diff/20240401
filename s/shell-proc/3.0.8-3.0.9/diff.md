# Comparing `tmp/shell_proc-3.0.8.tar.gz` & `tmp/shell_proc-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_proc-3.0.8.tar", last modified: Sun Mar 10 19:07:43 2024, max compression
+gzip compressed data, was "shell_proc-3.0.9.tar", last modified: Mon Apr  1 19:31:49 2024, max compression
```

## Comparing `shell_proc-3.0.8.tar` & `shell_proc-3.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 19:07:43.187977 shell_proc-3.0.8/
--rw-rw-rw-   0        0        0     1090 2023-08-11 20:46:49.000000 shell_proc-3.0.8/LICENSE
--rw-rw-rw-   0        0        0      579 2023-08-11 20:46:49.000000 shell_proc-3.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    12335 2024-03-10 19:07:43.186977 shell_proc-3.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11818 2023-11-21 09:24:36.000000 shell_proc-3.0.8/README.rst
--rw-rw-rw-   0        0        0        0 2023-08-11 20:46:49.000000 shell_proc-3.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-10 19:07:43.187977 shell_proc-3.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2940 2023-08-11 20:46:49.000000 shell_proc-3.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-10 19:07:43.183430 shell_proc-3.0.8/shell_proc/
--rw-rw-rw-   0        0        0      286 2023-11-21 08:55:43.000000 shell_proc-3.0.8/shell_proc/__init__.py
--rw-rw-rw-   0        0        0      777 2023-08-11 20:46:49.000000 shell_proc-3.0.8/shell_proc/__main__.py
--rw-rw-rw-   0        0        0      194 2024-03-10 19:07:08.000000 shell_proc-3.0.8/shell_proc/__meta__.py
--rw-rw-rw-   0        0        0     1554 2023-11-15 04:05:25.000000 shell_proc-3.0.8/shell_proc/non_blocking_pipe.py
--rw-rw-rw-   0        0        0    45767 2024-03-10 19:05:59.000000 shell_proc-3.0.8/shell_proc/shell.py
-drwxrwxrwx   0        0        0        0 2024-03-10 19:07:43.185560 shell_proc-3.0.8/shell_proc.egg-info/
--rw-rw-rw-   0        0        0    12335 2024-03-10 19:07:43.000000 shell_proc-3.0.8/shell_proc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-03-10 19:07:43.000000 shell_proc-3.0.8/shell_proc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 19:07:43.000000 shell_proc-3.0.8/shell_proc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-10 19:07:43.000000 shell_proc-3.0.8/shell_proc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 19:31:49.432583 shell_proc-3.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-08-11 20:46:49.000000 shell_proc-3.0.9/LICENSE
+-rw-rw-rw-   0        0        0      579 2023-08-11 20:46:49.000000 shell_proc-3.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    12335 2024-04-01 19:31:49.431582 shell_proc-3.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11818 2023-11-21 09:24:36.000000 shell_proc-3.0.9/README.rst
+-rw-rw-rw-   0        0        0        0 2023-08-11 20:46:49.000000 shell_proc-3.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:31:49.432583 shell_proc-3.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2940 2023-08-11 20:46:49.000000 shell_proc-3.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:31:49.428006 shell_proc-3.0.9/shell_proc/
+-rw-rw-rw-   0        0        0      286 2023-11-21 08:55:43.000000 shell_proc-3.0.9/shell_proc/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-08-11 20:46:49.000000 shell_proc-3.0.9/shell_proc/__main__.py
+-rw-rw-rw-   0        0        0      194 2024-04-01 19:30:45.000000 shell_proc-3.0.9/shell_proc/__meta__.py
+-rw-rw-rw-   0        0        0     1554 2023-11-15 04:05:25.000000 shell_proc-3.0.9/shell_proc/non_blocking_pipe.py
+-rw-rw-rw-   0        0        0    46096 2024-04-01 19:29:08.000000 shell_proc-3.0.9/shell_proc/shell.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:31:49.431582 shell_proc-3.0.9/shell_proc.egg-info/
+-rw-rw-rw-   0        0        0    12335 2024-04-01 19:31:49.000000 shell_proc-3.0.9/shell_proc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-01 19:31:49.000000 shell_proc-3.0.9/shell_proc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:31:49.000000 shell_proc-3.0.9/shell_proc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-01 19:31:49.000000 shell_proc-3.0.9/shell_proc.egg-info/top_level.txt
```

### Comparing `shell_proc-3.0.8/LICENSE` & `shell_proc-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_proc-3.0.8/MANIFEST.in` & `shell_proc-3.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `shell_proc-3.0.8/PKG-INFO` & `shell_proc-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shell_proc
-Version: 3.0.8
+Version: 3.0.9
 Summary: Continuous shell process
 Home-page: https://github.com/justengel/shell_proc
-Download-URL: https://github.com/justengel/shell_proc/archive/v3.0.8.tar.gz
+Download-URL: https://github.com/justengel/shell_proc/archive/v3.0.9.tar.gz
 Author: Justin Engel
 Author-email: jtengel08@gmail.com
 License: Proprietary
 Keywords: shell bash subprocess sh
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shell_proc-3.0.8/README.rst` & `shell_proc-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `shell_proc-3.0.8/setup.py` & `shell_proc-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `shell_proc-3.0.8/shell_proc/__main__.py` & `shell_proc-3.0.9/shell_proc/__main__.py`

 * *Files identical despite different names*

### Comparing `shell_proc-3.0.8/shell_proc/non_blocking_pipe.py` & `shell_proc-3.0.9/shell_proc/non_blocking_pipe.py`

 * *Files identical despite different names*

### Comparing `shell_proc-3.0.8/shell_proc/shell.py` & `shell_proc-3.0.9/shell_proc/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,18 @@
         """Add output data to the proper file/pipe handler."""
         if not pipe_name.startswith('std'):
             pipe_name = 'std' + pipe_name
 
         self._last_pipe_data_time = time.time()
         setattr(self, pipe_name, getattr(self, 'raw_' + pipe_name, '') + data)
 
+    def reset_last_read_timeout(self):
+        """Reset the last read data time."""
+        self._last_pipe_data_time = 0
+
     def last_read_timeout(self, timeout: float = 1.1):
         """Return if the last read data time is greater than or equal to the given timeout"""
         return self._last_pipe_data_time != 0 and (time.time() - self._last_pipe_data_time) >= timeout
 
     def has_output(self):
         """Return if this command has any stdout."""
         return bool(self.stdout)
@@ -468,16 +472,20 @@
     end_command = property(get_end_command, set_end_command)
     end_command_bytes = property(get_end_command_bytes, set_end_command)
 
     def get_echo_results_cmd(self):
         cmd = 'echo "{end_cmd} {report}"'.format(end_cmd=self.end_command, report='$?')
         return cmd.encode()
 
-    def echo_results(self):
+    def echo_results(self, reset_last_read_timeout: bool = True):
         """Send the echo command to find the results of the previous command."""
+        cmd = self.current_command
+        if reset_last_read_timeout and cmd is not None and not cmd.is_finished():
+            cmd.reset_last_read_timeout()
+
         echo = self.get_echo_results_cmd()
         self.proc.stdin.write(echo + self.NEWLINE_BYTES)
         self.proc.stdin.flush()
 
     def _run(self, cmd, pipe_text='', extra=b'', end=b'', echo_results=True, **kwargs):
         """Run the given text command."""
         if extra:
```

### Comparing `shell_proc-3.0.8/shell_proc.egg-info/PKG-INFO` & `shell_proc-3.0.9/shell_proc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shell-proc
-Version: 3.0.8
+Version: 3.0.9
 Summary: Continuous shell process
 Home-page: https://github.com/justengel/shell_proc
-Download-URL: https://github.com/justengel/shell_proc/archive/v3.0.8.tar.gz
+Download-URL: https://github.com/justengel/shell_proc/archive/v3.0.9.tar.gz
 Author: Justin Engel
 Author-email: jtengel08@gmail.com
 License: Proprietary
 Keywords: shell bash subprocess sh
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

