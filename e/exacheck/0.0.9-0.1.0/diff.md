# Comparing `tmp/exacheck-0.0.9.tar.gz` & `tmp/exacheck-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exacheck-0.0.9.tar", max compression
+gzip compressed data, was "exacheck-0.1.0.tar", max compression
```

## Comparing `exacheck-0.0.9.tar` & `exacheck-0.1.0.tar`

### file list

```diff
@@ -1,56 +1,54 @@
--rw-r--r--   0        0        0     1060 2024-01-29 07:09:39.881253 exacheck-0.0.9/LICENSE
--rw-r--r--   0        0        0     1813 2024-02-06 16:22:10.836429 exacheck-0.0.9/README.md
--rw-r--r--   0        0        0        0 2024-02-05 13:21:09.084737 exacheck-0.0.9/exacheck/__init__.py
--rw-r--r--   0        0        0      198 2024-02-06 16:22:20.120443 exacheck-0.0.9/exacheck/__version__.py
--rw-r--r--   0        0        0     9035 2024-02-06 16:22:28.956457 exacheck-0.0.9/exacheck/announcer.py
--rw-r--r--   0        0        0     5218 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/checkexecutor.py
--rw-r--r--   0        0        0     2413 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/checkresult.py
--rw-r--r--   0        0        0     1954 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/checkstate.py
--rw-r--r--   0        0        0     2693 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/cli.py
--rw-r--r--   0        0        0     7125 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/configuration.py
--rw-r--r--   0        0        0    17845 2024-02-06 16:22:28.956457 exacheck-0.0.9/exacheck/exacheck.py
--rw-r--r--   0        0        0        0 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/exceptions/__init__.py
--rw-r--r--   0        0        0      520 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/exceptions/addressfamilyerror.py
--rw-r--r--   0        0        0      397 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/exceptions/checktimeout.py
--rw-r--r--   0        0        0      447 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/exceptions/dnsresolutionerror.py
--rw-r--r--   0        0        0      449 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/exceptions/workerprocesserror.py
--rw-r--r--   0        0        0    11129 2024-02-06 16:23:29.960549 exacheck-0.0.9/exacheck/logmanager.py
--rw-r--r--   0        0        0      606 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/__init__.py
--rw-r--r--   0        0        0     1644 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/_base.py
--rw-r--r--   0        0        0    12642 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/_remote.py
--rw-r--r--   0        0        0     9523 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/dns.py
--rw-r--r--   0        0        0     2403 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/file.py
--rw-r--r--   0        0        0     7214 2024-02-06 16:49:40.505822 exacheck-0.0.9/exacheck/methods/http.py
--rw-r--r--   0        0        0      155 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/http_extra/__init__.py
--rw-r--r--   0        0        0     1504 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/http_extra/sniadapter.py
--rw-r--r--   0        0        0     7108 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/icmp.py
--rw-r--r--   0        0        0     6473 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/ntp.py
--rw-r--r--   0        0        0     2445 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/shell.py
--rw-r--r--   0        0        0     3485 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/methods/tcp.py
--rw-r--r--   0        0        0     7610 2024-02-06 16:22:20.124443 exacheck-0.0.9/exacheck/notifications.py
--rw-r--r--   0        0        0     2088 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/procname.py
--rw-r--r--   0        0        0        0 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/__init__.py
--rw-r--r--   0        0        0      528 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/_base.py
--rw-r--r--   0        0        0    10512 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/check.py
--rw-r--r--   0        0        0      589 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/__init__.py
--rw-r--r--   0        0        0      757 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/_base.py
--rw-r--r--   0        0        0     2217 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/_remote.py
--rw-r--r--   0        0        0     3969 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/dnsargs.py
--rw-r--r--   0        0        0     1351 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/fileargs.py
--rw-r--r--   0        0        0     7013 2024-02-06 16:23:29.960549 exacheck-0.0.9/exacheck/settings/checkargs/httpargs.py
--rw-r--r--   0        0        0     6955 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/icmpargs.py
--rw-r--r--   0        0        0     2166 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/ntpargs.py
--rw-r--r--   0        0        0      793 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/shellargs.py
--rw-r--r--   0        0        0     1477 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/checkargs/tcpargs.py
--rw-r--r--   0        0        0      764 2024-02-06 16:22:20.124443 exacheck-0.0.9/exacheck/settings/exacheck.py
--rw-r--r--   0        0        0      168 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/loggers/__init__.py
--rw-r--r--   0        0        0     2824 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/loggers/_base.py
--rw-r--r--   0        0        0     2795 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/loggers/logfile.py
--rw-r--r--   0        0        0     3251 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/loggers/syslog.py
--rw-r--r--   0        0        0     2750 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/settings/notifications.py
--rw-r--r--   0        0        0     1500 2024-02-06 16:22:28.956457 exacheck-0.0.9/exacheck/settings/sentry.py
--rw-r--r--   0        0        0     4560 2024-02-06 16:22:20.124443 exacheck-0.0.9/exacheck/settings/settings.py
--rw-r--r--   0        0        0     3222 2024-02-06 16:20:18.168247 exacheck-0.0.9/exacheck/sleeper.py
--rw-r--r--   0        0        0    13996 2024-02-06 16:22:28.956457 exacheck-0.0.9/exacheck/worker.py
--rw-r--r--   0        0        0     2772 2024-02-06 16:55:17.540417 exacheck-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     4293 1970-01-01 00:00:00.000000 exacheck-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-02-08 17:18:51.304656 exacheck-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1813 2024-02-08 17:18:51.304656 exacheck-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-05 13:21:09.084737 exacheck-0.1.0/exacheck/__init__.py
+-rw-r--r--   0        0        0      198 2024-02-06 16:22:20.120443 exacheck-0.1.0/exacheck/__version__.py
+-rw-r--r--   0        0        0     9035 2024-02-06 16:22:28.956457 exacheck-0.1.0/exacheck/announcer.py
+-rw-r--r--   0        0        0     5218 2024-02-21 08:10:52.814613 exacheck-0.1.0/exacheck/checkexecutor.py
+-rw-r--r--   0        0        0     2413 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/checkresult.py
+-rw-r--r--   0        0        0     1954 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/checkstate.py
+-rw-r--r--   0        0        0     2693 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/cli.py
+-rw-r--r--   0        0        0     7125 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/configuration.py
+-rw-r--r--   0        0        0    20989 2024-03-20 15:22:48.053436 exacheck-0.1.0/exacheck/exacheck.py
+-rw-r--r--   0        0        0        0 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/__init__.py
+-rw-r--r--   0        0        0      520 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/addressfamilyerror.py
+-rw-r--r--   0        0        0      397 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/checktimeout.py
+-rw-r--r--   0        0        0      447 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/dnsresolutionerror.py
+-rw-r--r--   0        0        0      449 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/workerprocesserror.py
+-rw-r--r--   0        0        0    11129 2024-03-31 09:25:23.028122 exacheck-0.1.0/exacheck/logmanager.py
+-rw-r--r--   0        0        0      606 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/__init__.py
+-rw-r--r--   0        0        0     1644 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/_base.py
+-rw-r--r--   0        0        0    12642 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/_remote.py
+-rw-r--r--   0        0        0     9523 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/dns.py
+-rw-r--r--   0        0        0     2403 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/file.py
+-rw-r--r--   0        0        0     8192 2024-04-01 15:42:37.124154 exacheck-0.1.0/exacheck/methods/http.py
+-rw-r--r--   0        0        0     7108 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/icmp.py
+-rw-r--r--   0        0        0     6473 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/ntp.py
+-rw-r--r--   0        0        0     2445 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/shell.py
+-rw-r--r--   0        0        0     3485 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/tcp.py
+-rw-r--r--   0        0        0     7610 2024-03-20 15:22:48.053436 exacheck-0.1.0/exacheck/notifications.py
+-rw-r--r--   0        0        0     2088 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/procname.py
+-rw-r--r--   0        0        0        0 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/__init__.py
+-rw-r--r--   0        0        0      528 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/_base.py
+-rw-r--r--   0        0        0    10512 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/check.py
+-rw-r--r--   0        0        0      589 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/__init__.py
+-rw-r--r--   0        0        0      757 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/_base.py
+-rw-r--r--   0        0        0     2217 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/_remote.py
+-rw-r--r--   0        0        0     3969 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/dnsargs.py
+-rw-r--r--   0        0        0     1351 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/fileargs.py
+-rw-r--r--   0        0        0     7165 2024-04-01 15:42:37.124154 exacheck-0.1.0/exacheck/settings/checkargs/httpargs.py
+-rw-r--r--   0        0        0     6955 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/icmpargs.py
+-rw-r--r--   0        0        0     2166 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/ntpargs.py
+-rw-r--r--   0        0        0      793 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/shellargs.py
+-rw-r--r--   0        0        0     1477 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/tcpargs.py
+-rw-r--r--   0        0        0      764 2024-02-06 16:22:20.124443 exacheck-0.1.0/exacheck/settings/exacheck.py
+-rw-r--r--   0        0        0      168 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/__init__.py
+-rw-r--r--   0        0        0     2824 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/_base.py
+-rw-r--r--   0        0        0     2795 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/logfile.py
+-rw-r--r--   0        0        0     3251 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/syslog.py
+-rw-r--r--   0        0        0     2750 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/notifications.py
+-rw-r--r--   0        0        0     1500 2024-02-06 16:22:28.956457 exacheck-0.1.0/exacheck/settings/sentry.py
+-rw-r--r--   0        0        0     4560 2024-02-06 16:22:20.124443 exacheck-0.1.0/exacheck/settings/settings.py
+-rw-r--r--   0        0        0     3222 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/sleeper.py
+-rw-r--r--   0        0        0    13996 2024-02-21 08:01:57.744512 exacheck-0.1.0/exacheck/worker.py
+-rw-r--r--   0        0        0     3320 2024-04-01 15:44:46.811009 exacheck-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 exacheck-0.1.0/PKG-INFO
```

### Comparing `exacheck-0.0.9/LICENSE` & `exacheck-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/README.md` & `exacheck-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/announcer.py` & `exacheck-0.1.0/exacheck/announcer.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/checkexecutor.py` & `exacheck-0.1.0/exacheck/checkexecutor.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/checkresult.py` & `exacheck-0.1.0/exacheck/checkresult.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/checkstate.py` & `exacheck-0.1.0/exacheck/checkstate.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/cli.py` & `exacheck-0.1.0/exacheck/cli.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/configuration.py` & `exacheck-0.1.0/exacheck/configuration.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/exacheck.py` & `exacheck-0.1.0/exacheck/exacheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 ExaCheck - ExaBGP Health Checker
 
 Main ExaCheck class
 """
 
 from __future__ import annotations
 
+from errno import ECHILD
 from multiprocessing import Process
+from os import waitpid, WNOHANG, kill
 from pathlib import Path
 from pprint import pformat
 from time import sleep
 from typing import Tuple, cast
-from signal import signal, SIGTERM, SIGINT
+from signal import signal, SIGTERM, SIGINT, SIGCHLD
 import sys
 import importlib.metadata
 
 from loguru import logger
 
 from .exceptions.workerprocesserror import WorkerProcessError
 from .logmanager import LogManager
@@ -109,14 +111,17 @@
             base=f"ExaCheck Master Process [{self.configuration.settings.file}]",
             log_context=self.log,
         )
 
         # Set process name
         self.procname.update(message="Starting workers")
 
+        # Create signal handler to handle zombie processes
+        signal(SIGCHLD, self._reap)
+
         # Create jobs
         self.jobs = self._start_processes()
 
         # Notify that ExaCheck is started
         self.notifications.notify(
             event="info",
             title="ExaCheck Startup",
@@ -157,16 +162,27 @@
             self.procname.update(message="Monitoring loop start")
 
             # Loop over each job defined in configuration
             self.log.bind(event="debug").debug(
                 "Looping over each worker to ensure it is alive"
             )
             for job in self.jobs:
+                # Get the PID of the job
+                pid = job[1].pid
+
+                # Make sure the PID exists/is running
+                try:
+                    kill(pid, 0)
+                except Exception:
+                    running = False
+                else:
+                    running = True
+
                 # Ensure that the job is still alive
-                if job[1].is_alive():
+                if job[1].is_alive() and running:
                     # Worker is alive; log it
                     self.log.bind(event="debug").trace(
                         "Worker '{job_name}' is alive", job_name=job[0].name
                     )
 
                 else:
                     # Worker is not alive; respawn it
@@ -216,14 +232,20 @@
                     )
 
             else:
                 self.log.bind(event="debug").trace(
                     "Live configuration reload disabled; not checking for modifications"
                 )
 
+            # Call waitpid in case of zombie processes hanging around
+            try:
+                waitpid(-1, WNOHANG)
+            except Exception:
+                pass
+
             # Finish the sleep timer
             sleeper.finish()
 
             # Set new process name
             self.procname.update(
                 message=f"Sleeping for {sleeper.sleep_time:.3f} seconds"
             )
@@ -507,7 +529,72 @@
         self.jobs.remove(worker)
 
         # Logging
         self.log.bind(event="info").info(
             "Check worker for '{name}' has been stopped",
             name=check.name,
         )
+
+    def _reap(self, signum, frame) -> None:
+        """Handly SIGCHLD signals to reap zombie processes"""
+        # Logging
+        self.log.bind(event="debug").info(
+            "Received SIGCHLD; reaping zombie processes"
+        )
+
+        try:
+            # Run in loop to catch any processes
+            while True:
+                # Run waitpid for process
+                pid, status = waitpid(-1, WNOHANG)
+                # Check if this is the main process
+                if pid == 0:
+                    # No more processes to reap
+                    self.log.bind(event="debug").debug(
+                        "Finished reaping processes"
+                    )
+                    break
+
+                # Get the exit code of process
+                code = status >> 8
+
+                # Log information about it
+                self.log.bind(event="debug").info(
+                    "Reaped process {pid} with exit code {code}",
+                    pid=pid,
+                    code=code,
+                )
+
+                # Respawn the check
+                for check, worker in self.jobs:
+                    if worker.pid == pid:
+                        self.log.bind(event="info").info(
+                            "Worker '{check_name}' has exited; it will be respawned",
+                            check_name=check.name,
+                        )
+
+                        # Create the new worker process
+                        new_worker = self._create_process(check=check)
+
+                        # Start the new worker
+                        new_worker.start()
+
+                        # Replace the job with the new one
+                        self.jobs[self.jobs.index((check, worker))] = (check, new_worker)
+
+                        # Send notification
+                        self.notifications.notify(
+                            event="error",
+                            title=f"ExaCheck Worker Failure - {check.name}",
+                            message=f"The ExaCheck worker process for the health check `{check.name}` failed and has now been respawned.",
+                        )
+
+        except OSError as exc:
+            if exc.errno == ECHILD:
+                self.log.bind(event="info").info(
+                    "No child processes to reap"
+                )
+            else:
+                self.log.bind(event="error").error(
+                    "Error reaping processes: {exc}",
+                    exc=exc,
+                )
```

### Comparing `exacheck-0.0.9/exacheck/exceptions/addressfamilyerror.py` & `exacheck-0.1.0/exacheck/exceptions/addressfamilyerror.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/logmanager.py` & `exacheck-0.1.0/exacheck/logmanager.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/__init__.py` & `exacheck-0.1.0/exacheck/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/_base.py` & `exacheck-0.1.0/exacheck/methods/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/_remote.py` & `exacheck-0.1.0/exacheck/methods/_remote.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/dns.py` & `exacheck-0.1.0/exacheck/methods/dns.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/file.py` & `exacheck-0.1.0/exacheck/methods/file.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/http.py` & `exacheck-0.1.0/exacheck/methods/http.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 Check Method - HTTP
 """
 
 import warnings
 from pprint import pformat
 from ipaddress import ip_address, IPv6Address
 
-import requests
+import httpx
 
 from ..checkresult import CheckResult
 from ..settings.checkargs.httpargs import HTTPArgs
-from .http_extra import SNIAdapter
 from ._remote import Remote
 
 
 class HTTP(Remote):
     """
     Run a HTTP health check
     """
@@ -26,30 +25,33 @@
     def check_one(self, addr: str) -> CheckResult:
         """
         Run the HTTP health check
         """
         # Set type for MyPy
         self.args: HTTPArgs
 
-        # Create the HTTP/S client session
-        session = self._create_session()
-
         # Send the HTTP request and get response
         try:
-            response = self._request(session=session, addr=addr)
+            response = self._request(addr=addr)
+        except httpx.ConnectError as exc:
+            return CheckResult(
+                success=False,
+                message="HTTP request connection error",
+                error=f"Connection error to {addr}: {exc}",
+            )
         except Exception as exc:
             return CheckResult(success=False, message=f"HTTP request failed: {exc}")
 
         # Perform validation on the response and get the check result object
         result = self._validate(response=response)
 
         # Return the check result
         return result
 
-    def _validate(self, response: requests.Response) -> CheckResult:
+    def _validate(self, response: httpx.Response) -> CheckResult:
         """
         Validate the HTTP response received
         """
         # Check if a specific response code is required; if so validate it matches
         if (
             self.args.expected_status
             and response.status_code not in self.args.expected_status
@@ -62,15 +64,15 @@
                     f"{', '.join(map(str, self.args.expected_status))}"
                 ),
             )
 
         # Check if a successful response code is required; if so validate it matches
         if (
             self.args.require_status
-            and response.status_code != requests.codes.ok  # pylint: disable=no-member
+            and response.status_code != httpx.codes.OK
         ):
             return CheckResult(
                 success=False,
                 message=f"HTTP status code {response.status_code} does not match expected status code(s)",
                 error=f"{response.status_code} could not be confirmed as a valid status code",
             )
 
@@ -85,62 +87,55 @@
         # Return a valid check result
         return CheckResult(
             success=True,
             message="HTTP response was valid and passed all checks",
             output=f"HTTP response received in {response.elapsed.total_seconds():.3f} seconds",
         )
 
-    def _request(self, session: requests.Session, addr: str) -> requests.Response:
+    def _request(self, addr: str) -> httpx.Response:
         """
         Send the HTTP request and return the response
         """
         # Get the URL to make request to
         url = self._create_url(addr=addr)
 
-        # Disable SSL warning if not verifying certificate
-        if self.args.url.scheme == "https" and not self.args.verify_ssl:
-            warnings.filterwarnings("ignore", message="Unverified HTTPS request")
-
-        # Send the request of the specified type
-        response = getattr(session, self.args.request_method.lower())(
-            url=url,
-            timeout=self.args.http_timeout,
-            params=self.args.url.query,
-            data=self.args.data,
-        )
-
-        # Return the response
-        return response
-
-    def _create_session(self) -> requests.Session:
-        """
-        Create the HTTP/S client session
-        """
-        # Create the client session
-        session = requests.Session()
-
         # Create the headers for the request
         headers = self._create_headers()
 
-        # Check if the URL is HTTPS and if the request is to a hostname
-        if self.args.url.scheme == "https" and "Host" in headers:
-            # Mount the SNI adapter for SNI support
-            session.mount("https://", SNIAdapter())
-
-        # Set the headers from "headers"
-        session.headers.update(headers)
+        # Set up authentication if required
+        authentication = self._create_auth()
 
-        # Set basic auth credentials if required
-        if self.args.url.username and self.args.url.password:
-            session.auth = (self.args.url.username, self.args.url.password)
+        # Get any extensions required
+        extensions = self._create_extensions()
 
-        # Set the SSL verification option if required
-        session.verify = self.args.verify_ssl
+        # Send the request of the appropriate type
+        with httpx.Client(
+            headers=headers,
+            verify=self.args.verify_ssl,
+            http2=self.args.http2,
+            timeout=self.args.http_timeout,
+            auth=authentication,
+        ) as client:
+            # If the request is a GET request, no data can be included
+            if self.args.request_method.lower() == "get":
+                response = client.get(
+                    url=url,
+                    params=self.args.url.query,
+                    extensions=extensions,
+                )
+            else:
+                response = getattr(client, self.args.request_method.lower())(
+                    url=url,
+                    params=self.args.url.query,
+                    data=self.args.data,
+                    extensions=extensions,
+                )
 
-        return session
+        # Return the response
+        return response
 
     def _create_headers(self) -> dict[str, str]:
         """
         Create the HTTP headers to use for the HTTP request
         """
         self.log.bind(event="debug").debug("Creating HTTP headers")
 
@@ -205,14 +200,53 @@
 
         # Log the URL that will be used
         self.log.bind(event="debug").debug("HTTP URL created: {url}", url=url)
 
         # Return the URL
         return url
 
+    def _create_auth(self) -> tuple[str, str] | None:
+        """
+        Set up a HTTP basic authentication object if required
+        """
+        # Only proceed if the username and password are set
+        if self.args.url.username and self.args.url.password:
+            # Return tuple of username/password
+            return (self.args.url.username, self.args.url.password)
+
+        # No auth configured
+        return None
+
+    def _create_extensions(self) -> dict[str, str] | None:
+        """
+        Set up any extensions required for the HTTP request
+
+        Currently this only configures SNI if required but this may be extended in future
+        """
+        # If the scheme is not HTTPS, skip
+        if self.args.url.scheme != "https":
+            return None
+
+        # If there is no host available, skip
+        if not self.args.url.host:
+            return None
+
+        # If the host is an IP address, skip
+        if self._is_ip(self.args.url.host):
+            return None
+
+        # Create empty dict of extensions
+        extensions: dict[str, str] = {}
+
+        # Set up the SNI extension
+        extensions["sni"] = self.args.url.host
+
+        # Return the extensions
+        return extensions
+
     # Check if the supplied value is an IP address
     @staticmethod
     def _is_ip(value: str) -> bool:
         """
         Check if the supplied value is an IP address
         """
         try:
```

### Comparing `exacheck-0.0.9/exacheck/methods/icmp.py` & `exacheck-0.1.0/exacheck/methods/icmp.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/ntp.py` & `exacheck-0.1.0/exacheck/methods/ntp.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/shell.py` & `exacheck-0.1.0/exacheck/methods/shell.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/methods/tcp.py` & `exacheck-0.1.0/exacheck/methods/tcp.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/notifications.py` & `exacheck-0.1.0/exacheck/notifications.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/procname.py` & `exacheck-0.1.0/exacheck/procname.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/_base.py` & `exacheck-0.1.0/exacheck/settings/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/check.py` & `exacheck-0.1.0/exacheck/settings/check.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/__init__.py` & `exacheck-0.1.0/exacheck/settings/checkargs/__init__.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/_base.py` & `exacheck-0.1.0/exacheck/settings/checkargs/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/_remote.py` & `exacheck-0.1.0/exacheck/settings/checkargs/_remote.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/dnsargs.py` & `exacheck-0.1.0/exacheck/settings/checkargs/dnsargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/fileargs.py` & `exacheck-0.1.0/exacheck/settings/checkargs/fileargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/httpargs.py` & `exacheck-0.1.0/exacheck/settings/checkargs/httpargs.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,20 @@
 
     data: Optional[dict[str, str]] = Field(
         title="Request Data",
         description="The request data to send for POST requests",
         default=None,
     )
 
+    http2: bool = Field(
+        title="Enable HTTP/2",
+        description="Enable the HTTP/2 protocol for the request",
+        default=False,
+    )
+
     @field_validator("http_timeout")
     # pylint: disable=no-self-argument
     def validate_http_timeout(
         cls, http_timeout: int | float, values: ValidationInfo
     ) -> int | float:
         """
         Ensure that the HTTP timeout is a valid value
```

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/icmpargs.py` & `exacheck-0.1.0/exacheck/settings/checkargs/icmpargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/ntpargs.py` & `exacheck-0.1.0/exacheck/settings/checkargs/ntpargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/shellargs.py` & `exacheck-0.1.0/exacheck/settings/checkargs/shellargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/checkargs/tcpargs.py` & `exacheck-0.1.0/exacheck/settings/checkargs/tcpargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/exacheck.py` & `exacheck-0.1.0/exacheck/settings/exacheck.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/loggers/_base.py` & `exacheck-0.1.0/exacheck/settings/loggers/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/loggers/logfile.py` & `exacheck-0.1.0/exacheck/settings/loggers/logfile.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/loggers/syslog.py` & `exacheck-0.1.0/exacheck/settings/loggers/syslog.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/notifications.py` & `exacheck-0.1.0/exacheck/settings/notifications.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/sentry.py` & `exacheck-0.1.0/exacheck/settings/sentry.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/settings/settings.py` & `exacheck-0.1.0/exacheck/settings/settings.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/sleeper.py` & `exacheck-0.1.0/exacheck/sleeper.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.0.9/exacheck/worker.py` & `exacheck-0.1.0/exacheck/worker.py`

 * *Files identical despite different names*

