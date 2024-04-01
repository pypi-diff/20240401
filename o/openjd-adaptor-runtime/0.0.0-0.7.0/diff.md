# Comparing `tmp/openjd-adaptor-runtime-0.0.0.tar.gz` & `tmp/openjd_adaptor_runtime-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjd-adaptor-runtime-0.0.0.tar", last modified: Fri Sep  1 03:50:04 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `openjd-adaptor-runtime-0.0.0.tar` & `openjd_adaptor_runtime-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,71 @@
-drwxr-xr-x   0 neilsd   (6731894) amazon     (100)        0 2023-09-01 03:50:04.426670 openjd-adaptor-runtime-0.0.0/
--rw-r--r--   0 neilsd   (6731894) amazon     (100)    11357 2023-09-01 03:41:25.000000 openjd-adaptor-runtime-0.0.0/LICENSE
--rw-r--r--   0 neilsd   (6731894) amazon     (100)      178 2023-09-01 03:50:04.426670 openjd-adaptor-runtime-0.0.0/PKG-INFO
--rw-r--r--   0 neilsd   (6731894) amazon     (100)       13 2023-09-01 03:43:24.000000 openjd-adaptor-runtime-0.0.0/README.md
--rw-r--r--   0 neilsd   (6731894) amazon     (100)      267 2023-09-01 03:49:48.000000 openjd-adaptor-runtime-0.0.0/pyproject.toml
--rw-r--r--   0 neilsd   (6731894) amazon     (100)       38 2023-09-01 03:50:04.426670 openjd-adaptor-runtime-0.0.0/setup.cfg
-drwxr-xr-x   0 neilsd   (6731894) amazon     (100)        0 2023-09-01 03:50:04.426670 openjd-adaptor-runtime-0.0.0/src/
-drwxr-xr-x   0 neilsd   (6731894) amazon     (100)        0 2023-09-01 03:50:04.426670 openjd-adaptor-runtime-0.0.0/src/openjd/
-drwxr-xr-x   0 neilsd   (6731894) amazon     (100)        0 2023-09-01 03:50:04.426670 openjd-adaptor-runtime-0.0.0/src/openjd/adaptor_runtime/
--rw-r--r--   0 neilsd   (6731894) amazon     (100)        0 2023-09-01 03:43:58.000000 openjd-adaptor-runtime-0.0.0/src/openjd/adaptor_runtime/__init__.py
-drwxr-xr-x   0 neilsd   (6731894) amazon     (100)        0 2023-09-01 03:50:04.426670 openjd-adaptor-runtime-0.0.0/src/openjd_adaptor_runtime.egg-info/
--rw-r--r--   0 neilsd   (6731894) amazon     (100)      178 2023-09-01 03:50:04.000000 openjd-adaptor-runtime-0.0.0/src/openjd_adaptor_runtime.egg-info/PKG-INFO
--rw-r--r--   0 neilsd   (6731894) amazon     (100)      271 2023-09-01 03:50:04.000000 openjd-adaptor-runtime-0.0.0/src/openjd_adaptor_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 neilsd   (6731894) amazon     (100)        1 2023-09-01 03:50:04.000000 openjd-adaptor-runtime-0.0.0/src/openjd_adaptor_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 neilsd   (6731894) amazon     (100)        7 2023-09-01 03:50:04.000000 openjd-adaptor-runtime-0.0.0/src/openjd_adaptor_runtime.egg-info/top_level.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/__init__.py
+-rw-r--r--   0        0        0    19313 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_entrypoint.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_osname.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_version.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/configuration.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/configuration.schema.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/py.typed
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/__init__.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/backend_named_pipe_server.py
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/backend_runner.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/background_named_pipe_request_handler.py
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/frontend_runner.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/http_server.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/log_buffers.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/model.py
+-rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/server_response.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/exceptions.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/request_handler.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/sockets.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/__init__.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/named_pipe_request_handler.py
+-rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/named_pipe_server.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/__init__.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/_logging.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/_secure_open.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/__init__.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor_runner.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor_states.py
+-rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_base_adaptor.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_command_adaptor.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_path_mapping.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_validator.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_versioning.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_adaptor_configuration.schema.json
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_configuration.py
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_configuration_manager.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/app_handlers/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/app_handlers/_regex_callback_handler.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/__init__.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_actions_queue.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_adaptor_server.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_adaptor_server_response.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_http_request_handler.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_named_pipe_request_handler.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_win_adaptor_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_logging.py
+-rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_logging_subprocess.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_managed_process.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_stream_logger.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/_version.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/action.py
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/base_client_interface.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/connection.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/posix_client_interface.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/py.typed
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/win_client_interface.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/named_pipe_config.py
+-rw-r--r--   0        0        0    17311 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/named_pipe_helper.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/NOTICE
+-rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/hatch.toml
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    11449 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/PKG-INFO
```

### Comparing `openjd-adaptor-runtime-0.0.0/LICENSE` & `openjd_adaptor_runtime-0.7.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -168,34 +169,7 @@
       or other liability obligations and/or rights consistent with this
       License. However, in accepting such obligations, You may act only
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
```

