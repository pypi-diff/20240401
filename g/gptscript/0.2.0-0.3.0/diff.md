# Comparing `tmp/gptscript-0.2.0.tar.gz` & `tmp/gptscript-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptscript-0.2.0.tar", last modified: Thu Mar 14 21:27:07 2024, max compression
+gzip compressed data, was "gptscript-0.3.0.tar", last modified: Mon Apr  1 18:42:39 2024, max compression
```

## Comparing `gptscript-0.2.0.tar` & `gptscript-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-03-14 21:27:07.069233 gptscript-0.2.0/
--rw-r--r--   0 wmaxwell   (501) staff       (20)    10175 2024-03-08 22:16:36.000000 gptscript-0.2.0/LICENSE
--rw-r--r--   0 wmaxwell   (501) staff       (20)    19246 2024-03-14 21:27:07.069028 gptscript-0.2.0/PKG-INFO
--rw-r--r--   0 wmaxwell   (501) staff       (20)     7032 2024-03-08 22:16:36.000000 gptscript-0.2.0/README.md
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-03-14 21:27:07.068034 gptscript-0.2.0/gptscript/
--rw-r--r--   0 wmaxwell   (501) staff       (20)        0 2024-03-08 22:16:36.000000 gptscript-0.2.0/gptscript/__init__.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     2782 2024-03-08 22:16:36.000000 gptscript-0.2.0/gptscript/command.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)      927 2024-03-08 22:16:36.000000 gptscript-0.2.0/gptscript/exec_utils.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     5452 2024-03-14 21:25:10.000000 gptscript-0.2.0/gptscript/install.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     1870 2024-03-08 22:16:36.000000 gptscript-0.2.0/gptscript/tool.py
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-03-14 21:27:07.068833 gptscript-0.2.0/gptscript.egg-info/
--rw-r--r--   0 wmaxwell   (501) staff       (20)    19246 2024-03-14 21:27:07.000000 gptscript-0.2.0/gptscript.egg-info/PKG-INFO
--rw-r--r--   0 wmaxwell   (501) staff       (20)      362 2024-03-14 21:27:07.000000 gptscript-0.2.0/gptscript.egg-info/SOURCES.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)        1 2024-03-14 21:27:07.000000 gptscript-0.2.0/gptscript.egg-info/dependency_links.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       64 2024-03-14 21:27:07.000000 gptscript-0.2.0/gptscript.egg-info/entry_points.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       99 2024-03-14 21:27:07.000000 gptscript-0.2.0/gptscript.egg-info/requires.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       10 2024-03-14 21:27:07.000000 gptscript-0.2.0/gptscript.egg-info/top_level.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)      802 2024-03-14 21:25:10.000000 gptscript-0.2.0/pyproject.toml
--rw-r--r--   0 wmaxwell   (501) staff       (20)       38 2024-03-14 21:27:07.069270 gptscript-0.2.0/setup.cfg
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-03-14 21:27:07.068705 gptscript-0.2.0/tests/
--rw-r--r--   0 wmaxwell   (501) staff       (20)     3232 2024-03-08 22:16:36.000000 gptscript-0.2.0/tests/test_gptscript.py
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.200501 gptscript-0.3.0/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    10175 2024-03-08 22:16:36.000000 gptscript-0.3.0/LICENSE
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    19246 2024-04-01 18:42:39.200240 gptscript-0.3.0/PKG-INFO
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     7032 2024-03-08 22:16:36.000000 gptscript-0.3.0/README.md
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.199283 gptscript-0.3.0/gptscript/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)        0 2024-03-08 22:16:36.000000 gptscript-0.3.0/gptscript/__init__.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     2782 2024-03-08 22:16:36.000000 gptscript-0.3.0/gptscript/command.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      927 2024-03-08 22:16:36.000000 gptscript-0.3.0/gptscript/exec_utils.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     5452 2024-03-14 21:25:10.000000 gptscript-0.3.0/gptscript/install.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     1867 2024-04-01 18:37:22.000000 gptscript-0.3.0/gptscript/tool.py
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.200070 gptscript-0.3.0/gptscript.egg-info/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    19246 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/PKG-INFO
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      362 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/SOURCES.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)        1 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/dependency_links.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       64 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/entry_points.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       99 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/requires.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       10 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/top_level.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      802 2024-04-01 18:37:22.000000 gptscript-0.3.0/pyproject.toml
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       38 2024-04-01 18:42:39.200533 gptscript-0.3.0/setup.cfg
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.199951 gptscript-0.3.0/tests/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     3232 2024-03-08 22:16:36.000000 gptscript-0.3.0/tests/test_gptscript.py
```

### Comparing `gptscript-0.2.0/LICENSE` & `gptscript-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gptscript-0.2.0/PKG-INFO` & `gptscript-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptscript
-Version: 0.2.0
+Version: 0.3.0
 Summary: Run gptscripts from Python apps
 Author-email: Bill Maxwell <bill@acorn.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gptscript-0.2.0/README.md` & `gptscript-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gptscript-0.2.0/gptscript/command.py` & `gptscript-0.3.0/gptscript/command.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.2.0/gptscript/exec_utils.py` & `gptscript-0.3.0/gptscript/exec_utils.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.2.0/gptscript/install.py` & `gptscript-0.3.0/gptscript/install.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.2.0/gptscript/tool.py` & `gptscript-0.3.0/gptscript/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         description="",
         tools=[],
         max_tokens=None,
         model="",
         cache=True,
         temperature=None,
         args={},
-        internal_prompt="",
+        internal_prompt=False,
         instructions="",
         json_response=False,
     ):
         self.name = name
         self.description = description
         self.tools = tools
         self.max_tokens = max_tokens
@@ -43,15 +43,15 @@
         if self.temperature is not None:
             tool += f"Temperature: {self.temperature}\n"
         if self.json_response:
             tool += "JSON Response: true\n"
         if self.args:
             for arg, desc in self.args.items():
                 tool += f"Args: {arg}: {desc}\n"
-        if self.internal_prompt != "":
+        if self.internal_prompt:
             tool += f"Internal prompt: {self.internal_prompt}\n"
         if self.instructions != "":
             tool += self.instructions
 
         return tool
```

### Comparing `gptscript-0.2.0/gptscript.egg-info/PKG-INFO` & `gptscript-0.3.0/gptscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptscript
-Version: 0.2.0
+Version: 0.3.0
 Summary: Run gptscripts from Python apps
 Author-email: Bill Maxwell <bill@acorn.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gptscript-0.2.0/pyproject.toml` & `gptscript-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.9.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gptscript"
-version = "0.2.0"
+version = "0.3.0"
 description = "Run gptscripts from Python apps"
 readme = "README.md"
 authors = [{ name = "Bill Maxwell", email = "bill@acorn.io" }]
 license = { file = "LICENSE" }
 dependencies = [
     "certifi==2024.2.2",
     "charset-normalizer==3.3.2",
```

### Comparing `gptscript-0.2.0/tests/test_gptscript.py` & `gptscript-0.3.0/tests/test_gptscript.py`

 * *Files identical despite different names*

