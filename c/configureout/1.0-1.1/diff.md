# Comparing `tmp/configureout-1.0.tar.gz` & `tmp/configureout-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configureout-1.0.tar", last modified: Mon Apr  1 12:50:55 2024, max compression
+gzip compressed data, was "configureout-1.1.tar", last modified: Mon Apr  1 14:57:08 2024, max compression
```

## Comparing `configureout-1.0.tar` & `configureout-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 12:50:55.891288 configureout-1.0/
--rw-rw-rw-   0        0        0     2193 2024-04-01 12:50:55.890290 configureout-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1792 2024-04-01 12:00:52.000000 configureout-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 12:50:55.882289 configureout-1.0/configureout/
--rw-rw-rw-   0        0        0      613 2024-04-01 12:31:28.000000 configureout-1.0/configureout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:50:55.889320 configureout-1.0/configureout.egg-info/
--rw-rw-rw-   0        0        0     2193 2024-04-01 12:50:55.000000 configureout-1.0/configureout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-04-01 12:50:55.000000 configureout-1.0/configureout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 12:50:55.000000 configureout-1.0/configureout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-01 12:50:55.000000 configureout-1.0/configureout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 12:50:55.000000 configureout-1.0/configureout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 12:50:55.891288 configureout-1.0/setup.cfg
--rw-rw-rw-   0        0        0      671 2024-04-01 12:50:14.000000 configureout-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:57:08.516528 configureout-1.1/
+-rw-rw-rw-   0        0        0     2193 2024-04-01 14:57:08.515529 configureout-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1792 2024-04-01 13:08:22.000000 configureout-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 14:57:08.507027 configureout-1.1/configureout/
+-rw-rw-rw-   0        0        0      923 2024-04-01 14:56:05.000000 configureout-1.1/configureout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:57:08.514529 configureout-1.1/configureout.egg-info/
+-rw-rw-rw-   0        0        0     2193 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-01 14:57:08.000000 configureout-1.1/configureout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:57:08.516528 configureout-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      671 2024-04-01 14:55:59.000000 configureout-1.1/setup.py
```

### Comparing `configureout-1.0/PKG-INFO` & `configureout-1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: configureout
-Version: 1.0
+Version: 1.1
 Summary: A simple configuration module
 Home-page: https://github.com/EightShift/configureout
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# ConfigureOut
+# configureout
 
-ConfigureOut is a lightweight Python module designed to simplify the process of loading and accessing configuration data from JSON files. It provides a simple and intuitive interface for managing configuration settings within your Python applications.
+Configureout is a lightweight Python module designed to simplify the process of loading and accessing configuration data from JSON files. It provides a simple and intuitive interface for managing configuration settings within your Python applications.
 
 ## Features
 
-- **Easy Configuration Loading:** ConfigureOut allows you to load configuration settings from JSON files with just a few lines of code.
+- **Easy Configuration Loading:** Configureout allows you to load configuration settings from JSON files with just a few lines of code.
 - **Nested Configuration Support:** Easily access nested configuration settings using dot notation.
 - **Flexible and Extensible:** The module can be easily extended to suit your specific needs, allowing for customization and flexibility.
-- **Pythonic Interface:** ConfigureOut provides a Pythonic interface for accessing configuration settings, making it easy to integrate into your projects.
+- **Pythonic Interface:** Configureout provides a Pythonic interface for accessing configuration settings, making it easy to integrate into your projects.
 
 ## Installation
 
-You can install ConfigureOut via pip:
+You can install configureout via pip:
 
 ```
 pip install configureout
 ```
 
 ## Usage
 
@@ -54,15 +54,15 @@
   },
   "logging": {
     "level": "info",
     "file_path": "/var/log/app.log"
   }
 }
 ```
-With ConfigureOut, you can easily load and access these settings in your Python code:
+With configureout, you can easily load and access these settings in your Python code:
 ```
 from configureout import Config
 
 config = Config("config.json")
 
 # Access database host
 print(config.database.host)
```

### Comparing `configureout-1.0/README.md` & `configureout-1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# ConfigureOut
+# configureout
 
-ConfigureOut is a lightweight Python module designed to simplify the process of loading and accessing configuration data from JSON files. It provides a simple and intuitive interface for managing configuration settings within your Python applications.
+Configureout is a lightweight Python module designed to simplify the process of loading and accessing configuration data from JSON files. It provides a simple and intuitive interface for managing configuration settings within your Python applications.
 
 ## Features
 
-- **Easy Configuration Loading:** ConfigureOut allows you to load configuration settings from JSON files with just a few lines of code.
+- **Easy Configuration Loading:** Configureout allows you to load configuration settings from JSON files with just a few lines of code.
 - **Nested Configuration Support:** Easily access nested configuration settings using dot notation.
 - **Flexible and Extensible:** The module can be easily extended to suit your specific needs, allowing for customization and flexibility.
-- **Pythonic Interface:** ConfigureOut provides a Pythonic interface for accessing configuration settings, making it easy to integrate into your projects.
+- **Pythonic Interface:** Configureout provides a Pythonic interface for accessing configuration settings, making it easy to integrate into your projects.
 
 ## Installation
 
-You can install ConfigureOut via pip:
+You can install configureout via pip:
 
 ```
 pip install configureout
 ```
 
 ## Usage
 
@@ -42,15 +42,15 @@
   },
   "logging": {
     "level": "info",
     "file_path": "/var/log/app.log"
   }
 }
 ```
-With ConfigureOut, you can easily load and access these settings in your Python code:
+With configureout, you can easily load and access these settings in your Python code:
 ```
 from configureout import Config
 
 config = Config("config.json")
 
 # Access database host
 print(config.database.host)
```

### Comparing `configureout-1.0/configureout.egg-info/PKG-INFO` & `configureout-1.1/configureout.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: configureout
-Version: 1.0
+Version: 1.1
 Summary: A simple configuration module
 Home-page: https://github.com/EightShift/configureout
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# ConfigureOut
+# configureout
 
-ConfigureOut is a lightweight Python module designed to simplify the process of loading and accessing configuration data from JSON files. It provides a simple and intuitive interface for managing configuration settings within your Python applications.
+Configureout is a lightweight Python module designed to simplify the process of loading and accessing configuration data from JSON files. It provides a simple and intuitive interface for managing configuration settings within your Python applications.
 
 ## Features
 
-- **Easy Configuration Loading:** ConfigureOut allows you to load configuration settings from JSON files with just a few lines of code.
+- **Easy Configuration Loading:** Configureout allows you to load configuration settings from JSON files with just a few lines of code.
 - **Nested Configuration Support:** Easily access nested configuration settings using dot notation.
 - **Flexible and Extensible:** The module can be easily extended to suit your specific needs, allowing for customization and flexibility.
-- **Pythonic Interface:** ConfigureOut provides a Pythonic interface for accessing configuration settings, making it easy to integrate into your projects.
+- **Pythonic Interface:** Configureout provides a Pythonic interface for accessing configuration settings, making it easy to integrate into your projects.
 
 ## Installation
 
-You can install ConfigureOut via pip:
+You can install configureout via pip:
 
 ```
 pip install configureout
 ```
 
 ## Usage
 
@@ -54,15 +54,15 @@
   },
   "logging": {
     "level": "info",
     "file_path": "/var/log/app.log"
   }
 }
 ```
-With ConfigureOut, you can easily load and access these settings in your Python code:
+With configureout, you can easily load and access these settings in your Python code:
 ```
 from configureout import Config
 
 config = Config("config.json")
 
 # Access database host
 print(config.database.host)
```

### Comparing `configureout-1.0/setup.py` & `configureout-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='configureout',
-    version='1.0',
+    version='1.1',
     description='A simple configuration module',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='EightShift',
     author_email='the8shift@gmail.com',
     url='https://github.com/EightShift/configureout',
     packages=find_packages(),
```

