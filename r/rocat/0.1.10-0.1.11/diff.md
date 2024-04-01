# Comparing `tmp/rocat-0.1.10.tar.gz` & `tmp/rocat-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.1.10.tar", last modified: Mon Apr  1 14:34:03 2024, max compression
+gzip compressed data, was "rocat-0.1.11.tar", last modified: Mon Apr  1 16:01:09 2024, max compression
```

## Comparing `rocat-0.1.10.tar` & `rocat-0.1.11.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:03.203628 rocat-0.1.10/
--rw-rw-rw-   0        0        0       28 2024-04-01 14:23:32.000000 rocat-0.1.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2024-04-01 14:34:03.203628 rocat-0.1.10/PKG-INFO
--rw-rw-rw-   0        0        0     1781 2024-04-01 14:11:47.000000 rocat-0.1.10/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:03.189529 rocat-0.1.10/rocat/
--rw-rw-rw-   0        0        0      240 2024-04-01 14:18:04.000000 rocat-0.1.10/rocat/__init__.py
--rw-rw-rw-   0        0        0      164 2024-04-01 14:18:03.000000 rocat-0.1.10/rocat/api_utils.py
--rw-rw-rw-   0        0        0      955 2024-04-01 14:18:01.000000 rocat-0.1.10/rocat/chatbot.py
--rw-rw-rw-   0        0        0      627 2024-04-01 14:18:00.000000 rocat-0.1.10/rocat/streamlit_app.py
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:03.203167 rocat-0.1.10/rocat.egg-info/
--rw-rw-rw-   0        0        0     2085 2024-04-01 14:34:03.000000 rocat-0.1.10/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-01 14:34:03.000000 rocat-0.1.10/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:34:03.000000 rocat-0.1.10/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 14:34:03.000000 rocat-0.1.10/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-01 14:34:03.000000 rocat-0.1.10/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 14:34:03.203628 rocat-0.1.10/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-04-01 14:33:14.000000 rocat-0.1.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.988465 rocat-0.1.11/
+-rw-rw-rw-   0        0        0       28 2024-04-01 16:00:53.000000 rocat-0.1.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     1332 2024-04-01 16:01:09.987464 rocat-0.1.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1028 2024-04-01 16:00:52.000000 rocat-0.1.11/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.973894 rocat-0.1.11/rocat/
+-rw-rw-rw-   0        0        0      133 2024-04-01 16:00:58.000000 rocat-0.1.11/rocat/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-04-01 16:00:57.000000 rocat-0.1.11/rocat/chatbot_app.py
+-rw-rw-rw-   0        0        0      888 2024-04-01 16:00:56.000000 rocat-0.1.11/rocat/chatbot_modules.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.986465 rocat-0.1.11/rocat.egg-info/
+-rw-rw-rw-   0        0        0     1332 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-01 16:01:09.000000 rocat-0.1.11/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:01:09.988465 rocat-0.1.11/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-04-01 16:00:49.000000 rocat-0.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:01:09.985465 rocat-0.1.11/test/
+-rw-rw-rw-   0        0        0      286 2024-04-01 15:56:26.000000 rocat-0.1.11/test/test.py
```

### Comparing `rocat-0.1.10/PKG-INFO` & `rocat-0.1.11/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.1.10
+Version: 0.1.11
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/root39293/rocat
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: streamlit
@@ -19,42 +19,14 @@
 
 ​```
 pip install rocat
 ​```
 
 ## Usage
 
-To use RoCat in your project, follow these steps:
-
-1. Import the necessary modules from the RoCat library:
-
-​```
-from rocat import ChatbotModule, create_app, run_app
-​```
-
-2. Create an instance of the `ChatbotModule` with your OpenAI API key:
-
-​```
-api_key = "YOUR_API_KEY"
-chatbot = ChatbotModule(api_key)
-​```
-
-3. Use the `generate_response` method to generate a response based on a user prompt:
-
-​```
-user_prompt = "What is the capital of France?"
-response = chatbot.generate_response(user_prompt)
-print(response)
-​```
-
-4. (Optional) If you want to customize the system prompt for the chatbot, use the `set_system_prompt` method:
-
-​```
-chatbot.set_system_prompt("You are a helpful travel assistant.")
-​```
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
 
 ## Contributing
```

### Comparing `rocat-0.1.10/README.md` & `rocat-0.1.11/rocat.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,32 @@
+Metadata-Version: 2.1
+Name: rocat
+Version: 0.1.11
+Summary: A simple and user-friendly library for AI services
+Home-page: https://github.com/root39293/rocat
+Author: YumetaLab
+Author-email: root@yumeta.kr
+Description-Content-Type: text/markdown
+Requires-Dist: openai
+Requires-Dist: streamlit
+
 # RoCat: A Simple and User-Friendly Library for AI Services
 
 RoCat is a Python library that provides a simple and user-friendly interface for integrating AI services into your projects.
 
 ## Installation
 
 You can install RoCat using pip:
 
 ​```
 pip install rocat
 ​```
 
 ## Usage
 
-To use RoCat in your project, follow these steps:
-
-1. Import the necessary modules from the RoCat library:
-
-​```
-from rocat import ChatbotModule, create_app, run_app
-​```
-
-2. Create an instance of the `ChatbotModule` with your OpenAI API key:
-
-​```
-api_key = "YOUR_API_KEY"
-chatbot = ChatbotModule(api_key)
-​```
-
-3. Use the `generate_response` method to generate a response based on a user prompt:
-
-​```
-user_prompt = "What is the capital of France?"
-response = chatbot.generate_response(user_prompt)
-print(response)
-​```
-
-4. (Optional) If you want to customize the system prompt for the chatbot, use the `set_system_prompt` method:
-
-​```
-chatbot.set_system_prompt("You are a helpful travel assistant.")
-​```
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
 
 ## Contributing
 
@@ -57,8 +40,8 @@
 
 ## Contact
 
 If you have any questions or inquiries, please contact the author:
 
 - Name: Faith6
 - Email: root@yumeta.kr
-- GitHub: [Yumeta-Lab](https://github.com/Yumeta-Lab)
+- GitHub: [Yumeta-Lab](https://github.com/Yumeta-Lab)
```

### Comparing `rocat-0.1.10/setup.py` & `rocat-0.1.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rocat",
-    version="0.1.10",
+    version="0.1.11",
     description="A simple and user-friendly library for AI services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="YumetaLab",
     author_email="root@yumeta.kr",
     url="https://github.com/root39293/rocat",
     packages=find_packages(exclude=["tests"]),
```

