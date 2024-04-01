# Comparing `tmp/p621-0.1.0.tar.gz` & `tmp/p621-0.1.1.tar.gz`

## Comparing `p621-0.1.0.tar` & `p621-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 p621-0.1.0/.pypirc
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/requests.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/posts/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/posts/classes.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 p621-0.1.0/src/p621/posts/interactions.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 p621-0.1.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 p621-0.1.0/LICENSE
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 p621-0.1.0/README.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 p621-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 p621-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 p621-0.1.1/.pypirc
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 p621-0.1.1/src/p621/__init__.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 p621-0.1.1/src/p621/requests.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 p621-0.1.1/src/p621/posts/__init__.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 p621-0.1.1/src/p621/posts/classes.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 p621-0.1.1/src/p621/posts/interactions.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 p621-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 p621-0.1.1/LICENSE
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 p621-0.1.1/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 p621-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 p621-0.1.1/PKG-INFO
```

### Comparing `p621-0.1.0/src/p621/posts/classes.py` & `p621-0.1.1/src/p621/posts/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,20 +71,13 @@
         self.parent: int = post['relationships']['parent_id']
         self.children: list[str] = post['relationships']['children']
 
         self.approver_id: int = post['approver_id']
         self.uploader_id: int = post['uploader_id']
 
     def download(self, path: str = None) -> None:
-        import urllib.request
-
-        target: str = str(self.id) + '.' + self.file.extension
-        if path:
-            target = path + '/' + target
-
-        url: str = self.file.url
-        urllib.request.urlretrieve(url, target)
+        from .interactions import download_post
+        download_post(self, path)
 
     def open(self) -> None:
-        import webbrowser
-        url: str = 'https://e621.net/posts/' + str(self.id)
-        webbrowser.open(url)
+        from .interactions import open_post
+        open_post(self)
```

### Comparing `p621-0.1.0/LICENSE` & `p621-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `p621-0.1.0/README.md` & `p621-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `p621-0.1.0/pyproject.toml` & `p621-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [project]
 name = "p621"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="I'd Eat Some Fish", email="ideatsomefish@gmail.com" },
 ]
 description = "an oversimplified wrapper and interactivity for the e621 API"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+]
+dependencies = [
+  "requests"
 ]
 
 [project.urls]
-Homepage = "https://github.com/IdEatSomeFish/p621"
+Repository = "https://github.com/IdEatSomeFish/p621"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `p621-0.1.0/PKG-INFO` & `p621-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: p621
-Version: 0.1.0
+Version: 0.1.1
 Summary: an oversimplified wrapper and interactivity for the e621 API
-Project-URL: Homepage, https://github.com/IdEatSomeFish/p621
+Project-URL: Repository, https://github.com/IdEatSomeFish/p621
 Author-email: I'd Eat Some Fish <ideatsomefish@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 **unfinished!**
 
 # p621
 an oversimplified wrapper and interactivity for the **e621** API
```

