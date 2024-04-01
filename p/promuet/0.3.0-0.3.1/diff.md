# Comparing `tmp/promuet-0.3.0.tar.gz` & `tmp/promuet-0.3.1.tar.gz`

## Comparing `promuet-0.3.0.tar` & `promuet-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 promuet-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 promuet-0.3.0/requirements.lock
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 promuet-0.3.0/src/promuet/__init__.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 promuet-0.3.0/src/promuet/ai_client.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 promuet-0.3.0/src/promuet/app_flow.py
--rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 promuet-0.3.0/src/promuet/match_items.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 promuet-0.3.0/src/promuet/prompt_flow.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 promuet-0.3.0/src/promuet/prompt_message.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 promuet-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 promuet-0.3.0/tests/test_match_items.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 promuet-0.3.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 promuet-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 promuet-0.3.0/README.md
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 promuet-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 promuet-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 promuet-0.3.1/requirements-dev.lock
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 promuet-0.3.1/requirements.lock
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 promuet-0.3.1/src/promuet/__init__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 promuet-0.3.1/src/promuet/ai_client.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 promuet-0.3.1/src/promuet/app_flow.py
+-rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 promuet-0.3.1/src/promuet/match_items.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 promuet-0.3.1/src/promuet/prompt_flow.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 promuet-0.3.1/src/promuet/prompt_message.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 promuet-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 promuet-0.3.1/tests/test_match_items.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 promuet-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 promuet-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 promuet-0.3.1/README.md
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 promuet-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 promuet-0.3.1/PKG-INFO
```

### Comparing `promuet-0.3.0/requirements-dev.lock` & `promuet-0.3.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/requirements.lock` & `promuet-0.3.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/src/promuet/__init__.py` & `promuet-0.3.1/src/promuet/__init__.py`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/src/promuet/ai_client.py` & `promuet-0.3.1/src/promuet/ai_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 class CachedChatClient(ChatClientBase):
     def __init__(self, cache_path: Path, client: ChatClientBase):
         self.cache_path = cache_path
         self.cache = json.loads(cache_path.read_text()) if cache_path.is_file() else {}
         self.client = client
-        self.cache = {}
 
     def predict(self, messages: list[dict]) -> str:
         key = md5(
             self.client.cache_key + json.dumps(messages, sort_keys=True).encode()
         ).hexdigest()
         if key not in self.cache:
             self.cache[key] = self.client.predict(messages)
```

### Comparing `promuet-0.3.0/src/promuet/app_flow.py` & `promuet-0.3.1/src/promuet/app_flow.py`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/src/promuet/match_items.py` & `promuet-0.3.1/src/promuet/match_items.py`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/src/promuet/prompt_flow.py` & `promuet-0.3.1/src/promuet/prompt_flow.py`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/src/promuet/prompt_message.py` & `promuet-0.3.1/src/promuet/prompt_message.py`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/tests/test_match_items.py` & `promuet-0.3.1/tests/test_match_items.py`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/LICENSE.txt` & `promuet-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/README.md` & `promuet-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `promuet-0.3.0/pyproject.toml` & `promuet-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promuet"
-version = "0.3.0"
+version = "0.3.1"
 description = 'A simple yet powerful prompt templating engine'
 readme = "README.md"
 requires-python = ">= 3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Matthew D. Scholefield", email = "matthew331199@gmail.com" },
```

### Comparing `promuet-0.3.0/PKG-INFO` & `promuet-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: promuet
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple yet powerful prompt templating engine
 Project-URL: Documentation, https://github.com/MatthewScholefield/promuet#readme
 Project-URL: Issues, https://github.com/MatthewScholefield/promuet/issues
 Project-URL: Source, https://github.com/MatthewScholefield/promuet
 Author-email: "Matthew D. Scholefield" <matthew331199@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

