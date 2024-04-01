# Comparing `tmp/zella-0.0.4.tar.gz` & `tmp/zella-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zella-0.0.4.tar", last modified: Wed Jan 10 13:28:27 2024, max compression
+gzip compressed data, was "zella-0.0.5.tar", last modified: Mon Apr  1 14:42:26 2024, max compression
```

## Comparing `zella-0.0.4.tar` & `zella-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.134497 zella-0.0.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1051 2024-01-10 11:57:14.000000 zella-0.0.4/LICENSE.md
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2597 2024-01-10 13:28:27.134497 zella-0.0.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2058 2024-01-10 11:57:14.000000 zella-0.0.4/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      685 2024-01-10 12:09:41.000000 zella-0.0.4/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-01-10 13:28:27.134497 zella-0.0.4/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.126497 zella-0.0.4/src/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      144 2024-01-10 11:57:14.000000 zella-0.0.4/src/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.130497 zella-0.0.4/src/zella/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1898 2024-01-10 12:09:26.000000 zella-0.0.4/src/zella/_client.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/config.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.130497 zella-0.0.4/src/zella/resources/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      188 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.130497 zella-0.0.4/src/zella/resources/callbacks/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/callbacks/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2841 2024-01-10 13:26:08.000000 zella-0.0.4/src/zella/resources/callbacks/langchain_callback.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.130497 zella-0.0.4/src/zella/resources/chat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/chat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      171 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/chat/chat.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1826 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/chat/completions.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.134497 zella-0.0.4/src/zella/resources/completions/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       37 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/completions/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1791 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/completions/completions.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.134497 zella-0.0.4/src/zella/resources/embedding/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/embedding/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1573 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/embedding/embedding.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.134497 zella-0.0.4/src/zella/resources/logger/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       26 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/logger/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1755 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/logger/log_consumer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1816 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/logger/logger.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.134497 zella-0.0.4/src/zella/resources/prompt/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       26 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/prompt/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1172 2024-01-10 11:57:14.000000 zella-0.0.4/src/zella/resources/prompt/prompt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       18 2024-01-10 13:27:21.000000 zella-0.0.4/src/zella/version.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-01-10 13:28:27.134497 zella-0.0.4/src/zella.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2597 2024-01-10 13:28:27.000000 zella-0.0.4/src/zella.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      916 2024-01-10 13:28:27.000000 zella-0.0.4/src/zella.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-01-10 13:28:27.000000 zella-0.0.4/src/zella.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2024-01-10 13:28:27.000000 zella-0.0.4/src/zella.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2024-01-10 13:28:27.000000 zella-0.0.4/src/zella.egg-info/top_level.txt
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.897596 zella-0.0.5/
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1051 2023-12-09 19:35:59.000000 zella-0.0.5/LICENSE.md
+-rw-r--r--   0 shivamrana   (501) staff       (20)     2597 2024-04-01 14:42:26.897215 zella-0.0.5/PKG-INFO
+-rw-r--r--   0 shivamrana   (501) staff       (20)     2058 2023-12-09 19:35:59.000000 zella-0.0.5/README.md
+-rw-r--r--   0 shivamrana   (501) staff       (20)      685 2024-01-10 12:38:21.000000 zella-0.0.5/pyproject.toml
+-rw-r--r--   0 shivamrana   (501) staff       (20)       38 2024-04-01 14:42:26.898669 zella-0.0.5/setup.cfg
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.856610 zella-0.0.5/src/
+-rw-r--r--   0 shivamrana   (501) staff       (20)      144 2023-12-09 19:35:59.000000 zella-0.0.5/src/__init__.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.863828 zella-0.0.5/src/zella/
+-rw-r--r--   0 shivamrana   (501) staff       (20)       28 2023-12-09 19:35:59.000000 zella-0.0.5/src/zella/__init__.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1898 2024-01-10 12:37:27.000000 zella-0.0.5/src/zella/_client.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)       79 2024-04-01 14:40:20.000000 zella-0.0.5/src/zella/config.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.871171 zella-0.0.5/src/zella/resources/
+-rw-r--r--   0 shivamrana   (501) staff       (20)      188 2023-12-20 20:45:37.000000 zella-0.0.5/src/zella/resources/__init__.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.873926 zella-0.0.5/src/zella/resources/callbacks/
+-rw-r--r--   0 shivamrana   (501) staff       (20)       50 2023-12-11 18:34:00.000000 zella-0.0.5/src/zella/resources/callbacks/__init__.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     2841 2024-04-01 14:07:29.000000 zella-0.0.5/src/zella/resources/callbacks/langchain_callback.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.877510 zella-0.0.5/src/zella/resources/chat/
+-rw-r--r--   0 shivamrana   (501) staff       (20)       22 2023-12-09 19:35:59.000000 zella-0.0.5/src/zella/resources/chat/__init__.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)      171 2023-12-09 19:35:59.000000 zella-0.0.5/src/zella/resources/chat/chat.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1826 2024-01-10 07:05:47.000000 zella-0.0.5/src/zella/resources/chat/completions.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.881734 zella-0.0.5/src/zella/resources/completions/
+-rw-r--r--   0 shivamrana   (501) staff       (20)       37 2023-12-20 20:43:39.000000 zella-0.0.5/src/zella/resources/completions/__init__.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1791 2024-01-10 07:24:11.000000 zella-0.0.5/src/zella/resources/completions/completions.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.885090 zella-0.0.5/src/zella/resources/embedding/
+-rw-r--r--   0 shivamrana   (501) staff       (20)       32 2023-12-10 16:56:24.000000 zella-0.0.5/src/zella/resources/embedding/__init__.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1573 2024-01-10 07:05:47.000000 zella-0.0.5/src/zella/resources/embedding/embedding.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.891250 zella-0.0.5/src/zella/resources/logger/
+-rw-r--r--   0 shivamrana   (501) staff       (20)       26 2023-12-10 16:55:23.000000 zella-0.0.5/src/zella/resources/logger/__init__.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1755 2023-12-12 11:07:03.000000 zella-0.0.5/src/zella/resources/logger/log_consumer.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1802 2024-04-01 14:40:23.000000 zella-0.0.5/src/zella/resources/logger/logger.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.894178 zella-0.0.5/src/zella/resources/prompt/
+-rw-r--r--   0 shivamrana   (501) staff       (20)       26 2023-12-10 16:56:24.000000 zella-0.0.5/src/zella/resources/prompt/__init__.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)     1172 2023-12-10 16:56:24.000000 zella-0.0.5/src/zella/resources/prompt/prompt.py
+-rw-r--r--   0 shivamrana   (501) staff       (20)       18 2024-04-01 14:41:42.000000 zella-0.0.5/src/zella/version.py
+drwxr-xr-x   0 shivamrana   (501) staff       (20)        0 2024-04-01 14:42:26.895891 zella-0.0.5/src/zella.egg-info/
+-rw-r--r--   0 shivamrana   (501) staff       (20)     2597 2024-04-01 14:42:26.000000 zella-0.0.5/src/zella.egg-info/PKG-INFO
+-rw-r--r--   0 shivamrana   (501) staff       (20)      916 2024-04-01 14:42:26.000000 zella-0.0.5/src/zella.egg-info/SOURCES.txt
+-rw-r--r--   0 shivamrana   (501) staff       (20)        1 2024-04-01 14:42:26.000000 zella-0.0.5/src/zella.egg-info/dependency_links.txt
+-rw-r--r--   0 shivamrana   (501) staff       (20)       12 2024-04-01 14:42:26.000000 zella-0.0.5/src/zella.egg-info/requires.txt
+-rw-r--r--   0 shivamrana   (501) staff       (20)       15 2024-04-01 14:42:26.000000 zella-0.0.5/src/zella.egg-info/top_level.txt
```

### Comparing `zella-0.0.4/LICENSE.md` & `zella-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/PKG-INFO` & `zella-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zella
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for accessing Zella AI for building AI apps
 Author-email: Team Zella <dev@zella.ai>
 Project-URL: Homepage, https://github.com/ZellaAI/zella-py
 Project-URL: Issues, https://github.com/ZellaAI/zella-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zella-0.0.4/README.md` & `zella-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/pyproject.toml` & `zella-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella/_client.py` & `zella-0.0.5/src/zella/_client.py`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella/resources/callbacks/langchain_callback.py` & `zella-0.0.5/src/zella/resources/callbacks/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella/resources/chat/completions.py` & `zella-0.0.5/src/zella/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella/resources/completions/completions.py` & `zella-0.0.5/src/zella/resources/completions/completions.py`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella/resources/embedding/embedding.py` & `zella-0.0.5/src/zella/resources/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella/resources/logger/log_consumer.py` & `zella-0.0.5/src/zella/resources/logger/log_consumer.py`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella/resources/logger/logger.py` & `zella-0.0.5/src/zella/resources/logger/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 class Logger:
     def __init__(self, client, batch_logging):
         self.client = client
         self.log_consumer = LogConsumer(client) if batch_logging else None
         self.batch_logging = batch_logging
         pass
 
-    def log(self, action, request, response, platform, model, **kwargs):
+    def log(self, messages, output, model, **kwargs):
         """
         Log a request to Zella.
 
         Args:
-            action (str): Action type of the request [Eg, chat.completions, embedding].
-            request (str): Request sent to the platform.
-            response (str): Response received to the platform.
-            platform (str): Platform name.
-            model (str): Model name.
+            messages (str): Request sent to the platform.
+            output (str): Response received to the platform.
+            model (str): Model details.
             **kwargs: Additional arguments for prompt retrieval. Valid arguments are:
                 - token_usage (dict, optional): Dictionary of token usage details.
                     - prompt_tokens (int): Prompt tokens.
                     - completion_tokens (int): Completion tokens.
                     - total_tokens (int): Total tokens.
                 - meta (dict, optional): Dictionary of optional metadata to be logged.
 
         """
         log_request = {
-            "action": action,
-            "request": request,
-            "response": response,
-            "platform": platform,
-            "model": model,
+            "input": messages,
+            "output": output,
+            "model": model
         }
         if kwargs.get("user"):
             log_request["user"] = kwargs.get("user")
+        if kwargs.get("tags"):
+            log_request["tags"] = kwargs.get("tags")
+        if kwargs.get("message_chain_id"):
+            log_request["message_chain_id"] = kwargs.get("message_chain_id")
         if kwargs.get("meta"):
             log_request["meta"] = kwargs.get("meta")
         if kwargs.get("token_usage"):
             log_request["token_usage"] = kwargs.get("token_usage")
 
         if self.batch_logging:
             self.log_consumer.consume(log_request)
```

### Comparing `zella-0.0.4/src/zella/resources/prompt/prompt.py` & `zella-0.0.5/src/zella/resources/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `zella-0.0.4/src/zella.egg-info/PKG-INFO` & `zella-0.0.5/src/zella.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zella
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for accessing Zella AI for building AI apps
 Author-email: Team Zella <dev@zella.ai>
 Project-URL: Homepage, https://github.com/ZellaAI/zella-py
 Project-URL: Issues, https://github.com/ZellaAI/zella-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zella-0.0.4/src/zella.egg-info/SOURCES.txt` & `zella-0.0.5/src/zella.egg-info/SOURCES.txt`

 * *Files identical despite different names*

