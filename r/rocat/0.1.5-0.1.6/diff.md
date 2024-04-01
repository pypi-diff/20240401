# Comparing `tmp/rocat-0.1.5.tar.gz` & `tmp/rocat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.1.5.tar", last modified: Mon Apr  1 12:13:58 2024, max compression
+gzip compressed data, was "rocat-0.1.6.tar", last modified: Mon Apr  1 12:18:24 2024, max compression
```

## Comparing `rocat-0.1.5.tar` & `rocat-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 12:13:58.181899 rocat-0.1.5/
--rw-rw-rw-   0        0        0     2084 2024-04-01 12:13:58.180900 rocat-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1781 2024-04-01 11:40:02.000000 rocat-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 12:13:58.154315 rocat-0.1.5/ai_modules/
--rw-rw-rw-   0        0        0       99 2024-04-01 12:11:28.000000 rocat-0.1.5/ai_modules/__init__.py
--rw-rw-rw-   0        0        0      966 2024-04-01 12:13:24.000000 rocat-0.1.5/ai_modules/chatbot.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:13:58.180900 rocat-0.1.5/rocat.egg-info/
--rw-rw-rw-   0        0        0     2084 2024-04-01 12:13:58.000000 rocat-0.1.5/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-01 12:13:58.000000 rocat-0.1.5/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 12:13:58.000000 rocat-0.1.5/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 12:13:58.000000 rocat-0.1.5/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 12:13:58.000000 rocat-0.1.5/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 12:13:58.181899 rocat-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-04-01 12:13:27.000000 rocat-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:13:58.179508 rocat-0.1.5/utils/
--rw-rw-rw-   0        0        0      189 2024-04-01 11:40:02.000000 rocat-0.1.5/utils/__init__.py
--rw-rw-rw-   0        0        0      170 2024-04-01 12:04:22.000000 rocat-0.1.5/utils/api_utils.py
--rw-rw-rw-   0        0        0      629 2024-04-01 12:04:22.000000 rocat-0.1.5/utils/app_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:18:24.767096 rocat-0.1.6/
+-rw-rw-rw-   0        0        0     2084 2024-04-01 12:18:24.766492 rocat-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1781 2024-04-01 11:40:02.000000 rocat-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 12:18:24.765093 rocat-0.1.6/rocat.egg-info/
+-rw-rw-rw-   0        0        0     2084 2024-04-01 12:18:24.000000 rocat-0.1.6/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2024-04-01 12:18:24.000000 rocat-0.1.6/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:18:24.000000 rocat-0.1.6/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-01 12:18:24.000000 rocat-0.1.6/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:18:24.000000 rocat-0.1.6/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 12:18:24.767096 rocat-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-04-01 12:17:59.000000 rocat-0.1.6/setup.py
```

### Comparing `rocat-0.1.5/PKG-INFO` & `rocat-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/root39293/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: streamlit
```

### Comparing `rocat-0.1.5/README.md` & `rocat-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rocat-0.1.5/rocat.egg-info/PKG-INFO` & `rocat-0.1.6/rocat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/root39293/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: streamlit
```

### Comparing `rocat-0.1.5/setup.py` & `rocat-0.1.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rocat",
-    version="0.1.5",
+    version="0.1.6",
     description="A simple and user-friendly library for AI services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="YumetaLab",
     author_email="root@yumeta.kr",
     url="https://github.com/root39293/rocat",
     packages=find_packages(exclude=["tests"]),
```

