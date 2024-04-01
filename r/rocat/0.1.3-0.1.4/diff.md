# Comparing `tmp/rocat-0.1.3.tar.gz` & `tmp/rocat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.1.3.tar", last modified: Mon Apr  1 11:58:55 2024, max compression
+gzip compressed data, was "rocat-0.1.4.tar", last modified: Mon Apr  1 12:06:02 2024, max compression
```

## Comparing `rocat-0.1.3.tar` & `rocat-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:58:55.479865 rocat-0.1.3/
--rw-rw-rw-   0        0        0     2084 2024-04-01 11:58:55.478865 rocat-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1781 2024-04-01 11:40:02.000000 rocat-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 11:58:55.454763 rocat-0.1.3/ai_modules/
--rw-rw-rw-   0        0        0       99 2024-04-01 11:40:02.000000 rocat-0.1.3/ai_modules/__init__.py
--rw-rw-rw-   0        0        0      966 2024-04-01 11:41:01.000000 rocat-0.1.3/ai_modules/chatbot.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:58:55.477865 rocat-0.1.3/rocat.egg-info/
--rw-rw-rw-   0        0        0     2084 2024-04-01 11:58:55.000000 rocat-0.1.3/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-01 11:58:55.000000 rocat-0.1.3/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 11:58:55.000000 rocat-0.1.3/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 11:58:55.000000 rocat-0.1.3/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 11:58:55.000000 rocat-0.1.3/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 11:58:55.479865 rocat-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-04-01 11:58:48.000000 rocat-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:58:55.476865 rocat-0.1.3/utils/
--rw-rw-rw-   0        0        0      189 2024-04-01 11:40:02.000000 rocat-0.1.3/utils/__init__.py
--rw-rw-rw-   0        0        0      170 2024-04-01 11:40:02.000000 rocat-0.1.3/utils/api_utils.py
--rw-rw-rw-   0        0        0      629 2024-04-01 11:40:02.000000 rocat-0.1.3/utils/app_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:06:02.887446 rocat-0.1.4/
+-rw-rw-rw-   0        0        0     2084 2024-04-01 12:06:02.885672 rocat-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1781 2024-04-01 11:40:02.000000 rocat-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 12:06:02.862562 rocat-0.1.4/ai_modules/
+-rw-rw-rw-   0        0        0       99 2024-04-01 11:40:02.000000 rocat-0.1.4/ai_modules/__init__.py
+-rw-rw-rw-   0        0        0      966 2024-04-01 12:05:05.000000 rocat-0.1.4/ai_modules/chatbot.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:06:02.882791 rocat-0.1.4/rocat.egg-info/
+-rw-rw-rw-   0        0        0     2084 2024-04-01 12:06:02.000000 rocat-0.1.4/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-01 12:06:02.000000 rocat-0.1.4/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:06:02.000000 rocat-0.1.4/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-01 12:06:02.000000 rocat-0.1.4/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-01 12:06:02.000000 rocat-0.1.4/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 12:06:02.887446 rocat-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-04-01 12:03:40.000000 rocat-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:06:02.882791 rocat-0.1.4/utils/
+-rw-rw-rw-   0        0        0      189 2024-04-01 11:40:02.000000 rocat-0.1.4/utils/__init__.py
+-rw-rw-rw-   0        0        0      170 2024-04-01 12:04:22.000000 rocat-0.1.4/utils/api_utils.py
+-rw-rw-rw-   0        0        0      629 2024-04-01 12:04:22.000000 rocat-0.1.4/utils/app_utils.py
```

### Comparing `rocat-0.1.3/PKG-INFO` & `rocat-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/root39293/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: streamlit
```

### Comparing `rocat-0.1.3/README.md` & `rocat-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rocat-0.1.3/ai_modules/chatbot.py` & `rocat-0.1.4/ai_modules/chatbot.py`

 * *Files identical despite different names*

### Comparing `rocat-0.1.3/rocat.egg-info/PKG-INFO` & `rocat-0.1.4/rocat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/root39293/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: streamlit
```

### Comparing `rocat-0.1.3/setup.py` & `rocat-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rocat",
-    version="0.1.3",
+    version="0.1.4",
     description="A simple and user-friendly library for AI services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="YumetaLab",
     author_email="root@yumeta.kr",
     url="https://github.com/root39293/rocat",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `rocat-0.1.3/utils/app_utils.py` & `rocat-0.1.4/utils/app_utils.py`

 * *Files identical despite different names*

