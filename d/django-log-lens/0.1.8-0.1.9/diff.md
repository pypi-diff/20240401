# Comparing `tmp/django-log-lens-0.1.8.tar.gz` & `tmp/django-log-lens-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-log-lens-0.1.8.tar", last modified: Wed Mar 27 09:13:20 2024, max compression
+gzip compressed data, was "django-log-lens-0.1.9.tar", last modified: Mon Apr  1 14:27:02 2024, max compression
```

## Comparing `django-log-lens-0.1.8.tar` & `django-log-lens-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 09:13:20.669703 django-log-lens-0.1.8/
--rw-rw-rw-   0        0        0     1089 2024-03-21 09:18:32.000000 django-log-lens-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      174 2024-03-21 13:12:51.000000 django-log-lens-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3901 2024-03-27 09:13:20.669703 django-log-lens-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3193 2024-03-27 09:10:56.000000 django-log-lens-0.1.8/README.md
--rw-rw-rw-   0        0        0       24 2024-03-27 09:12:28.000000 django-log-lens-0.1.8/VERSION.json
-drwxrwxrwx   0        0        0        0 2024-03-27 09:13:20.614808 django-log-lens-0.1.8/django_log_lens/
--rw-rw-rw-   0        0        0       71 2024-03-26 07:13:51.000000 django-log-lens-0.1.8/django_log_lens/__init__.py
--rw-rw-rw-   0        0        0      204 2024-03-24 12:51:40.000000 django-log-lens-0.1.8/django_log_lens/apps.py
-drwxrwxrwx   0        0        0        0 2024-03-27 09:13:20.575720 django-log-lens-0.1.8/django_log_lens/static/
-drwxrwxrwx   0        0        0        0 2024-03-27 09:13:20.652928 django-log-lens-0.1.8/django_log_lens/static/django_log_lens/
--rw-rw-rw-   0        0        0     1052 2024-03-27 07:17:36.000000 django-log-lens-0.1.8/django_log_lens/static/django_log_lens/favicon-cyan.svg
--rw-rw-rw-   0        0        0     1052 2024-03-26 20:20:17.000000 django-log-lens-0.1.8/django_log_lens/static/django_log_lens/favicon.svg
--rw-rw-rw-   0        0        0     3465 2024-03-27 07:17:36.000000 django-log-lens-0.1.8/django_log_lens/static/django_log_lens/logger.js
--rw-rw-rw-   0        0        0     1504 2024-03-27 07:40:05.000000 django-log-lens-0.1.8/django_log_lens/static/django_log_lens/logo.svg
--rw-rw-rw-   0        0        0    27612 2024-03-26 15:48:58.000000 django-log-lens-0.1.8/django_log_lens/static/django_log_lens/script.js
--rw-rw-rw-   0        0        0     5541 2024-03-27 07:17:36.000000 django-log-lens-0.1.8/django_log_lens/static/django_log_lens/styles.css
-drwxrwxrwx   0        0        0        0 2024-03-27 09:13:20.669703 django-log-lens-0.1.8/django_log_lens/templates/
--rw-rw-rw-   0        0        0      184 2024-03-25 13:37:01.000000 django-log-lens-0.1.8/django_log_lens/templates/js-logger.html
--rw-rw-rw-   0        0        0     1591 2024-03-27 07:17:36.000000 django-log-lens-0.1.8/django_log_lens/templates/log-lens-login.html
--rw-rw-rw-   0        0        0     4403 2024-03-27 07:17:36.000000 django-log-lens-0.1.8/django_log_lens/templates/log-lens.html
--rw-rw-rw-   0        0        0      857 2024-03-26 07:10:02.000000 django-log-lens-0.1.8/django_log_lens/urls.py
--rw-rw-rw-   0        0        0     5614 2024-03-26 07:14:16.000000 django-log-lens-0.1.8/django_log_lens/views.py
-drwxrwxrwx   0        0        0        0 2024-03-27 09:13:20.630775 django-log-lens-0.1.8/django_log_lens.egg-info/
--rw-rw-rw-   0        0        0     3901 2024-03-27 09:13:20.000000 django-log-lens-0.1.8/django_log_lens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      752 2024-03-27 09:13:20.000000 django-log-lens-0.1.8/django_log_lens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 09:13:20.000000 django-log-lens-0.1.8/django_log_lens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-27 09:13:20.000000 django-log-lens-0.1.8/django_log_lens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      150 2024-03-27 09:13:20.675872 django-log-lens-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1186 2024-03-23 15:44:32.000000 django-log-lens-0.1.8/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-01 14:27:02.772343 django-log-lens-0.1.9/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1069 2024-03-28 14:30:30.000000 django-log-lens-0.1.9/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      168 2024-03-30 07:36:39.000000 django-log-lens-0.1.9/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3888 2024-04-01 14:27:02.772343 django-log-lens-0.1.9/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3099 2024-03-30 06:57:01.000000 django-log-lens-0.1.9/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       23 2024-03-30 10:24:28.000000 django-log-lens-0.1.9/VERSION.json
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-01 14:27:02.772343 django-log-lens-0.1.9/django_log_lens/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2024-03-28 14:30:30.000000 django-log-lens-0.1.9/django_log_lens/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      197 2024-03-28 14:30:30.000000 django-log-lens-0.1.9/django_log_lens/apps.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-01 14:27:02.768343 django-log-lens-0.1.9/django_log_lens/static/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-01 14:27:02.772343 django-log-lens-0.1.9/django_log_lens/static/django_log_lens/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1004 2024-03-28 14:30:30.000000 django-log-lens-0.1.9/django_log_lens/static/django_log_lens/favicon.svg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4548 2024-03-30 10:09:01.000000 django-log-lens-0.1.9/django_log_lens/static/django_log_lens/logger.js
+-rw-rw-r--   0 martin    (1000) martin    (1000)    26864 2024-03-29 16:34:16.000000 django-log-lens-0.1.9/django_log_lens/static/django_log_lens/logo.svg
+-rw-rw-r--   0 martin    (1000) martin    (1000)    26783 2024-03-28 18:41:26.000000 django-log-lens-0.1.9/django_log_lens/static/django_log_lens/script.js
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5396 2024-03-29 16:57:38.000000 django-log-lens-0.1.9/django_log_lens/static/django_log_lens/styles.css
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-01 14:27:02.772343 django-log-lens-0.1.9/django_log_lens/templates/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      180 2024-03-30 10:09:01.000000 django-log-lens-0.1.9/django_log_lens/templates/js-logger.html
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1569 2024-03-29 16:44:39.000000 django-log-lens-0.1.9/django_log_lens/templates/log-lens-login.html
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4573 2024-03-29 16:44:54.000000 django-log-lens-0.1.9/django_log_lens/templates/log-lens.html
+-rw-rw-r--   0 martin    (1000) martin    (1000)      837 2024-03-28 19:22:46.000000 django-log-lens-0.1.9/django_log_lens/urls.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5699 2024-03-29 17:02:05.000000 django-log-lens-0.1.9/django_log_lens/views.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-01 14:27:02.772343 django-log-lens-0.1.9/django_log_lens.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3888 2024-04-01 14:27:02.000000 django-log-lens-0.1.9/django_log_lens.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      734 2024-04-01 14:27:02.000000 django-log-lens-0.1.9/django_log_lens.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-04-01 14:27:02.000000 django-log-lens-0.1.9/django_log_lens.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       12 2024-04-01 14:27:02.000000 django-log-lens-0.1.9/django_log_lens.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       16 2024-04-01 14:27:02.000000 django-log-lens-0.1.9/django_log_lens.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      136 2024-04-01 14:27:02.772343 django-log-lens-0.1.9/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1385 2024-03-30 08:05:24.000000 django-log-lens-0.1.9/setup.py
```

### Comparing `django-log-lens-0.1.8/PKG-INFO` & `django-log-lens-0.1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,118 @@
-Metadata-Version: 2.1
-Name: django-log-lens
-Version: 0.1.8
-Summary: A lightweight Django app for viewing and managing log data conveniently
-Home-page: https://github.com/martinbroede/django-log-lens
-Author: Martin Broede
-Author-email: martin.broede@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[![PyPi](https://img.shields.io/badge/PyPi-django--log--lens-blue)](https://pypi.org/project/django-log-lens/)
-[![Version](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmartinbroede%2Fdjango-log-lens%2Fmain%2FVERSION.json&query=version&label=Latest%20Version)](https://raw.githubusercontent.com/martinbroede/django-log-lens/main/VERSION.json)
-[![linting](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml/badge.svg)](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml)
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-
-<br>
-
-<img width="830px" src="https://raw.githubusercontent.com/martinbroede/django-log-lens/main/django_log_lens/static/django_log_lens/logo.svg">
-
-<br>
-
-Django Log Lens is a Django app that provides a simple, lightweight and easy-to-use logging system for your Django project.
-
-
-## Getting Started
-
-### 1. Install `django-log-lens` from PyPi
-
-```
-pip install django-log-lens
-```
-
-### 2. Add `django_log_lens` to your `INSTALLED_APPS`
-
-```python
-# file: settings.py
-
-INSTALLED_APPS = [
-    'django_log_lens',
-    ...
-]
-```
-
-### 3. Add URL patterns to your `urls.py`
-
-```python
-# file: urls.py
-from django.urls import include
-
-urlpatterns = [
-    path('logs/', include('django_log_lens.urls')),
-    ...
-]
-```
-
-### 4. Add a `LOGGING` configuration in your `settings.py`
-
-Follow the instructions from the [official Django documentation](https://docs.djangoproject.com/en/5.0/topics/logging/#configuring-logging) to configure the logging system or use the example below.
-
-```python
-# file: settings.py
-from django_log_lens import LOG_FORMAT
-
-LOG_FOLDER = BASE_DIR / "logs"
-
-if not os.path.exists(LOG_FOLDER):
-    os.makedirs(LOG_FOLDER)
-
-LOGGING = {
-    "version": 1,
-    "disable_existing_loggers": False,
-    "formatters": {"default": {"format": LOG_FORMAT}},
-    "handlers": {
-        "log_collector": {
-            "level": "WARNING",
-            "class": "logging.FileHandler",
-            "filename": str(LOG_FOLDER / "collector.log"),
-            "formatter": "default",
-        },
-        "client_logger": {
-            "level": "DEBUG",
-            "class": "logging.FileHandler",
-            "filename": str(LOG_FOLDER / "client.log"),
-            "formatter": "default",
-        },
-    },
-    "loggers": {
-        "django_log_lens.client": {"handlers": ["client_logger"], "level": "DEBUG", "propagate": True},
-        "django" : {"handlers": ["log_collector"], "level": "DEBUG", "propagate": True},
-    }
-}
-
-ALLOW_JS_LOGGING = True  # django_log_lens setting: allows clients to send console logs to the server
-```
-
-### 5. Visit Log Lens
-
-You can now visit Django Log Lens by navigating to `{% url 'django_log_lens:view' %}` (code for your template) -
- if you configured the URL pattern as shown above, this would be `logs/view`
-
-
-## Third Party Licenses
-
-This project uses the Dracula theme by Zeno Rocha which is
-licensed under the [MIT License](https://raw.githubusercontent.com/dracula/dracula-theme/main/LICENSE)
+Metadata-Version: 2.1
+Name: django-log-lens
+Version: 0.1.9
+Summary: A lightweight Django app for viewing and managing log data conveniently
+Home-page: https://github.com/martinbroede/django-log-lens
+Author: Martin Broede
+Author-email: martin.broede@gmail.com
+Maintainer: Martin Broede
+Maintainer-email: martin.broede@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![PyPI](https://img.shields.io/badge/PyPI-django--log--lens-blue)](https://pypi.org/project/django-log-lens/)
+[![Version](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmartinbroede%2Fdjango-log-lens%2Fmain%2FVERSION.json&query=version&label=Latest%20Version)](https://raw.githubusercontent.com/martinbroede/django-log-lens/main/VERSION.json)
+[![linting](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml/badge.svg)](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+<br>
+
+<img width="830px" src="https://raw.githubusercontent.com/martinbroede/django-log-lens/main/django_log_lens/static/django_log_lens/logo.svg">
+
+<br>
+
+Django Log Lens is a Django app that provides a simple, lightweight and easy-to-use logging system for your Django project.
+
+
+## Getting Started
+
+### 1. Install `django-log-lens` from PyPI
+
+```
+pip install django-log-lens
+```
+
+### 2. Add `django_log_lens` to your `INSTALLED_APPS`
+
+```python
+# file: settings.py
+
+INSTALLED_APPS = [
+    'django_log_lens',
+    ...
+]
+```
+
+### 3. Add URL patterns to your `urls.py`
+
+```python
+# file: urls.py
+from django.urls import include
+
+urlpatterns = [
+    path('logs/', include('django_log_lens.urls')),
+    ...
+]
+```
+
+### 4. Add a `LOGGING` configuration in your `settings.py`
+
+Follow the instructions from the [official Django documentation](https://docs.djangoproject.com/en/5.0/topics/logging/#configuring-logging) to configure the logging system or use the example below.
+
+```python
+# file: settings.py
+from django_log_lens import LOG_FORMAT
+
+LOG_FOLDER = BASE_DIR / "logs"
+
+if not os.path.exists(LOG_FOLDER):
+    os.makedirs(LOG_FOLDER)
+
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "formatters": {"default": {"format": LOG_FORMAT}},
+    "handlers": {
+        "log_collector": {
+            "level": "WARNING",
+            "class": "logging.FileHandler",
+            "filename": str(LOG_FOLDER / "collector.log"),
+            "formatter": "default",
+        },
+        "client_logger": {
+            "level": "DEBUG",
+            "class": "logging.FileHandler",
+            "filename": str(LOG_FOLDER / "client.log"),
+            "formatter": "default",
+        },
+    },
+    "loggers": {
+        "django_log_lens.client": {"handlers": ["client_logger"], "level": "DEBUG", "propagate": True},
+        "django" : {"handlers": ["log_collector"], "level": "DEBUG", "propagate": True},
+    }
+}
+
+ALLOW_JS_LOGGING = True  # django_log_lens setting: allows clients to send console logs to the server
+```
+
+### 5. Visit Log Lens
+
+You can now visit Django Log Lens by navigating to `{% url 'django_log_lens:view' %}` (code for your template) -
+ if you configured the URL pattern as shown above, this would be `logs/view`
+
+
+## Third Party Licenses
+
+This project uses the Dracula theme by Zeno Rocha which is
+licensed under the [MIT License](https://raw.githubusercontent.com/dracula/dracula-theme/main/LICENSE)
+
```

### Comparing `django-log-lens-0.1.8/README.md` & `django-log-lens-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-[![PyPi](https://img.shields.io/badge/PyPi-django--log--lens-blue)](https://pypi.org/project/django-log-lens/)
-[![Version](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmartinbroede%2Fdjango-log-lens%2Fmain%2FVERSION.json&query=version&label=Latest%20Version)](https://raw.githubusercontent.com/martinbroede/django-log-lens/main/VERSION.json)
-[![linting](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml/badge.svg)](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml)
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-
-<br>
-
-<img width="830px" src="https://raw.githubusercontent.com/martinbroede/django-log-lens/main/django_log_lens/static/django_log_lens/logo.svg">
-
-<br>
-
-Django Log Lens is a Django app that provides a simple, lightweight and easy-to-use logging system for your Django project.
-
-
-## Getting Started
-
-### 1. Install `django-log-lens` from PyPi
-
-```
-pip install django-log-lens
-```
-
-### 2. Add `django_log_lens` to your `INSTALLED_APPS`
-
-```python
-# file: settings.py
-
-INSTALLED_APPS = [
-    'django_log_lens',
-    ...
-]
-```
-
-### 3. Add URL patterns to your `urls.py`
-
-```python
-# file: urls.py
-from django.urls import include
-
-urlpatterns = [
-    path('logs/', include('django_log_lens.urls')),
-    ...
-]
-```
-
-### 4. Add a `LOGGING` configuration in your `settings.py`
-
-Follow the instructions from the [official Django documentation](https://docs.djangoproject.com/en/5.0/topics/logging/#configuring-logging) to configure the logging system or use the example below.
-
-```python
-# file: settings.py
-from django_log_lens import LOG_FORMAT
-
-LOG_FOLDER = BASE_DIR / "logs"
-
-if not os.path.exists(LOG_FOLDER):
-    os.makedirs(LOG_FOLDER)
-
-LOGGING = {
-    "version": 1,
-    "disable_existing_loggers": False,
-    "formatters": {"default": {"format": LOG_FORMAT}},
-    "handlers": {
-        "log_collector": {
-            "level": "WARNING",
-            "class": "logging.FileHandler",
-            "filename": str(LOG_FOLDER / "collector.log"),
-            "formatter": "default",
-        },
-        "client_logger": {
-            "level": "DEBUG",
-            "class": "logging.FileHandler",
-            "filename": str(LOG_FOLDER / "client.log"),
-            "formatter": "default",
-        },
-    },
-    "loggers": {
-        "django_log_lens.client": {"handlers": ["client_logger"], "level": "DEBUG", "propagate": True},
-        "django" : {"handlers": ["log_collector"], "level": "DEBUG", "propagate": True},
-    }
-}
-
-ALLOW_JS_LOGGING = True  # django_log_lens setting: allows clients to send console logs to the server
-```
-
-### 5. Visit Log Lens
-
-You can now visit Django Log Lens by navigating to `{% url 'django_log_lens:view' %}` (code for your template) -
- if you configured the URL pattern as shown above, this would be `logs/view`
-
-
-## Third Party Licenses
-
-This project uses the Dracula theme by Zeno Rocha which is
+[![PyPI](https://img.shields.io/badge/PyPI-django--log--lens-blue)](https://pypi.org/project/django-log-lens/)
+[![Version](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmartinbroede%2Fdjango-log-lens%2Fmain%2FVERSION.json&query=version&label=Latest%20Version)](https://raw.githubusercontent.com/martinbroede/django-log-lens/main/VERSION.json)
+[![linting](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml/badge.svg)](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+<br>
+
+<img width="830px" src="https://raw.githubusercontent.com/martinbroede/django-log-lens/main/django_log_lens/static/django_log_lens/logo.svg">
+
+<br>
+
+Django Log Lens is a Django app that provides a simple, lightweight and easy-to-use logging system for your Django project.
+
+
+## Getting Started
+
+### 1. Install `django-log-lens` from PyPI
+
+```
+pip install django-log-lens
+```
+
+### 2. Add `django_log_lens` to your `INSTALLED_APPS`
+
+```python
+# file: settings.py
+
+INSTALLED_APPS = [
+    'django_log_lens',
+    ...
+]
+```
+
+### 3. Add URL patterns to your `urls.py`
+
+```python
+# file: urls.py
+from django.urls import include
+
+urlpatterns = [
+    path('logs/', include('django_log_lens.urls')),
+    ...
+]
+```
+
+### 4. Add a `LOGGING` configuration in your `settings.py`
+
+Follow the instructions from the [official Django documentation](https://docs.djangoproject.com/en/5.0/topics/logging/#configuring-logging) to configure the logging system or use the example below.
+
+```python
+# file: settings.py
+from django_log_lens import LOG_FORMAT
+
+LOG_FOLDER = BASE_DIR / "logs"
+
+if not os.path.exists(LOG_FOLDER):
+    os.makedirs(LOG_FOLDER)
+
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "formatters": {"default": {"format": LOG_FORMAT}},
+    "handlers": {
+        "log_collector": {
+            "level": "WARNING",
+            "class": "logging.FileHandler",
+            "filename": str(LOG_FOLDER / "collector.log"),
+            "formatter": "default",
+        },
+        "client_logger": {
+            "level": "DEBUG",
+            "class": "logging.FileHandler",
+            "filename": str(LOG_FOLDER / "client.log"),
+            "formatter": "default",
+        },
+    },
+    "loggers": {
+        "django_log_lens.client": {"handlers": ["client_logger"], "level": "DEBUG", "propagate": True},
+        "django" : {"handlers": ["log_collector"], "level": "DEBUG", "propagate": True},
+    }
+}
+
+ALLOW_JS_LOGGING = True  # django_log_lens setting: allows clients to send console logs to the server
+```
+
+### 5. Visit Log Lens
+
+You can now visit Django Log Lens by navigating to `{% url 'django_log_lens:view' %}` (code for your template) -
+ if you configured the URL pattern as shown above, this would be `logs/view`
+
+
+## Third Party Licenses
+
+This project uses the Dracula theme by Zeno Rocha which is
 licensed under the [MIT License](https://raw.githubusercontent.com/dracula/dracula-theme/main/LICENSE)
```

### Comparing `django-log-lens-0.1.8/django_log_lens/static/django_log_lens/favicon-cyan.svg` & `django-log-lens-0.1.9/django_log_lens/static/django_log_lens/favicon.svg`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,63 @@
-00000000: 3c73 7667 0d0a 2020 786d 6c6e 733d 2268  <svg..  xmlns="h
-00000010: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
-00000020: 2f32 3030 302f 7376 6722 0d0a 2020 786d  /2000/svg"..  xm
-00000030: 6c6e 733a 786c 696e 6b3d 2268 7474 703a  lns:xlink="http:
-00000040: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
-00000050: 392f 786c 696e 6b22 0d0a 2020 7665 7273  9/xlink"..  vers
-00000060: 696f 6e3d 2231 2e31 220d 0a20 2077 6964  ion="1.1"..  wid
-00000070: 7468 3d22 3332 7078 220d 0a20 2068 6569  th="32px"..  hei
-00000080: 6768 743d 2233 3270 7822 0d0a 2020 7669  ght="32px"..  vi
-00000090: 6577 426f 783d 222d 302e 3520 2d30 2e35  ewBox="-0.5 -0.5
-000000a0: 2031 3937 2031 3937 223e 0d0a 2020 3c64   197 197">..  <d
-000000b0: 6566 732f 3e0d 0a20 203c 673e 0d0a 2020  efs/>..  <g>..  
-000000c0: 2020 3c65 6c6c 6970 7365 0d0a 2020 2020    <ellipse..    
-000000d0: 2020 6378 3d22 3938 2e35 220d 0a20 2020    cx="98.5"..   
-000000e0: 2020 2063 793d 2239 382e 3522 0d0a 2020     cy="98.5"..  
-000000f0: 2020 2020 7278 3d22 3836 2e35 220d 0a20      rx="86.5".. 
-00000100: 2020 2020 2072 793d 2238 362e 3522 0d0a       ry="86.5"..
-00000110: 2020 2020 2020 6669 6c6c 3d22 2332 3232        fill="#222
-00000120: 3632 6522 0d0a 2020 2020 2020 7374 726f  62e"..      stro
-00000130: 6b65 3d22 6e6f 6e65 220d 0a20 2020 2020  ke="none"..     
-00000140: 2070 6f69 6e74 6572 2d65 7665 6e74 733d   pointer-events=
-00000150: 2261 6c6c 222f 3e0d 0a20 2020 203c 7061  "all"/>..    <pa
-00000160: 7468 0d0a 2020 2020 2020 643d 224d 2031  th..      d="M 1
-00000170: 3238 2039 3820 4c20 3338 2039 3822 0d0a  28 98 L 38 98"..
-00000180: 2020 2020 2020 6669 6c6c 3d22 6e6f 6e65        fill="none
-00000190: 220d 0a20 2020 2020 2073 7472 6f6b 653d  "..      stroke=
-000001a0: 2223 6666 3535 3535 220d 0a20 2020 2020  "#ff5555"..     
-000001b0: 2073 7472 6f6b 652d 7769 6474 683d 2232   stroke-width="2
-000001c0: 3422 0d0a 2020 2020 2020 7374 726f 6b65  4"..      stroke
-000001d0: 2d6d 6974 6572 6c69 6d69 743d 2231 3022  -miterlimit="10"
-000001e0: 0d0a 2020 2020 2020 706f 696e 7465 722d  ..      pointer-
-000001f0: 6576 656e 7473 3d22 7374 726f 6b65 222f  events="stroke"/
-00000200: 3e0d 0a20 2020 203c 7061 7468 0d0a 2020  >..    <path..  
-00000210: 2020 2020 643d 224d 2031 3738 2031 3338      d="M 178 138
-00000220: 204c 2033 3820 3133 3822 0d0a 2020 2020   L 38 138"..    
-00000230: 2020 6669 6c6c 3d22 6e6f 6e65 220d 0a20    fill="none".. 
-00000240: 2020 2020 2073 7472 6f6b 653d 2223 6666       stroke="#ff
-00000250: 6238 3663 220d 0a20 2020 2020 2073 7472  b86c"..      str
-00000260: 6f6b 652d 7769 6474 683d 2232 3422 0d0a  oke-width="24"..
-00000270: 2020 2020 2020 7374 726f 6b65 2d6d 6974        stroke-mit
-00000280: 6572 6c69 6d69 743d 2231 3022 0d0a 2020  erlimit="10"..  
-00000290: 2020 2020 706f 696e 7465 722d 6576 656e      pointer-even
-000002a0: 7473 3d22 7374 726f 6b65 222f 3e0d 0a20  ts="stroke"/>.. 
-000002b0: 2020 203c 7061 7468 0d0a 2020 2020 2020     <path..      
-000002c0: 643d 224d 2031 3438 2035 3820 4c20 3338  d="M 148 58 L 38
-000002d0: 2035 3822 0d0a 2020 2020 2020 6669 6c6c   58"..      fill
-000002e0: 3d22 6e6f 6e65 220d 0a20 2020 2020 2073  ="none"..      s
-000002f0: 7472 6f6b 653d 2223 3530 6661 3762 220d  troke="#50fa7b".
-00000300: 0a20 2020 2020 2073 7472 6f6b 652d 7769  .      stroke-wi
-00000310: 6474 683d 2232 3422 0d0a 2020 2020 2020  dth="24"..      
-00000320: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00000330: 743d 2231 3022 0d0a 2020 2020 2020 706f  t="10"..      po
-00000340: 696e 7465 722d 6576 656e 7473 3d22 7374  inter-events="st
-00000350: 726f 6b65 222f 3e0d 0a20 2020 203c 656c  roke"/>..    <el
-00000360: 6c69 7073 650d 0a20 2020 2020 2063 783d  lipse..      cx=
-00000370: 2239 382e 3522 0d0a 2020 2020 2020 6379  "98.5"..      cy
-00000380: 3d22 3938 2e35 220d 0a20 2020 2020 2072  ="98.5"..      r
-00000390: 783d 2238 362e 3522 0d0a 2020 2020 2020  x="86.5"..      
-000003a0: 7279 3d22 3836 2e35 220d 0a20 2020 2020  ry="86.5"..     
-000003b0: 2066 696c 6c3d 2223 3030 3030 220d 0a20   fill="#0000".. 
-000003c0: 2020 2020 2073 7472 6f6b 653d 2223 3862       stroke="#8b
-000003d0: 6539 6664 220d 0a20 2020 2020 2073 7472  e9fd"..      str
-000003e0: 6f6b 652d 7769 6474 683d 2232 3422 0d0a  oke-width="24"..
-000003f0: 2020 2020 2020 706f 696e 7465 722d 6576        pointer-ev
-00000400: 656e 7473 3d22 616c 6c22 2f3e 0d0a 2020  ents="all"/>..  
-00000410: 3c2f 673e 0d0a 3c2f 7376 673e            </g>..</svg>
+00000000: 3c73 7667 0a20 2078 6d6c 6e73 3d22 6874  <svg.  xmlns="ht
+00000010: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000020: 3230 3030 2f73 7667 220a 2020 786d 6c6e  2000/svg".  xmln
+00000030: 733a 786c 696e 6b3d 2268 7474 703a 2f2f  s:xlink="http://
+00000040: 7777 772e 7733 2e6f 7267 2f31 3939 392f  www.w3.org/1999/
+00000050: 786c 696e 6b22 0a20 2076 6572 7369 6f6e  xlink".  version
+00000060: 3d22 312e 3122 0a20 2077 6964 7468 3d22  ="1.1".  width="
+00000070: 3332 7078 220a 2020 6865 6967 6874 3d22  32px".  height="
+00000080: 3332 7078 220a 2020 7669 6577 426f 783d  32px".  viewBox=
+00000090: 222d 302e 3520 2d30 2e35 2031 3937 2031  "-0.5 -0.5 197 1
+000000a0: 3937 223e 0a20 203c 6465 6673 2f3e 0a20  97">.  <defs/>. 
+000000b0: 203c 673e 0a20 2020 203c 656c 6c69 7073   <g>.    <ellips
+000000c0: 650a 2020 2020 2020 6378 3d22 3938 2e35  e.      cx="98.5
+000000d0: 220a 2020 2020 2020 6379 3d22 3938 2e35  ".      cy="98.5
+000000e0: 220a 2020 2020 2020 7278 3d22 3836 2e35  ".      rx="86.5
+000000f0: 220a 2020 2020 2020 7279 3d22 3836 2e35  ".      ry="86.5
+00000100: 220a 2020 2020 2020 6669 6c6c 3d22 2332  ".      fill="#2
+00000110: 3232 3632 6522 0a20 2020 2020 2073 7472  2262e".      str
+00000120: 6f6b 653d 226e 6f6e 6522 0a20 2020 2020  oke="none".     
+00000130: 2070 6f69 6e74 6572 2d65 7665 6e74 733d   pointer-events=
+00000140: 2261 6c6c 222f 3e0a 2020 2020 3c70 6174  "all"/>.    <pat
+00000150: 680a 2020 2020 2020 643d 224d 2031 3238  h.      d="M 128
+00000160: 2039 3820 4c20 3338 2039 3822 0a20 2020   98 L 38 98".   
+00000170: 2020 2066 696c 6c3d 226e 6f6e 6522 0a20     fill="none". 
+00000180: 2020 2020 2073 7472 6f6b 653d 2223 6666       stroke="#ff
+00000190: 3535 3535 220a 2020 2020 2020 7374 726f  5555".      stro
+000001a0: 6b65 2d77 6964 7468 3d22 3234 220a 2020  ke-width="24".  
+000001b0: 2020 2020 7374 726f 6b65 2d6d 6974 6572      stroke-miter
+000001c0: 6c69 6d69 743d 2231 3022 0a20 2020 2020  limit="10".     
+000001d0: 2070 6f69 6e74 6572 2d65 7665 6e74 733d   pointer-events=
+000001e0: 2273 7472 6f6b 6522 2f3e 0a20 2020 203c  "stroke"/>.    <
+000001f0: 7061 7468 0a20 2020 2020 2064 3d22 4d20  path.      d="M 
+00000200: 3137 3820 3133 3820 4c20 3338 2031 3338  178 138 L 38 138
+00000210: 220a 2020 2020 2020 6669 6c6c 3d22 6e6f  ".      fill="no
+00000220: 6e65 220a 2020 2020 2020 7374 726f 6b65  ne".      stroke
+00000230: 3d22 2366 6662 3836 6322 0a20 2020 2020  ="#ffb86c".     
+00000240: 2073 7472 6f6b 652d 7769 6474 683d 2232   stroke-width="2
+00000250: 3422 0a20 2020 2020 2073 7472 6f6b 652d  4".      stroke-
+00000260: 6d69 7465 726c 696d 6974 3d22 3130 220a  miterlimit="10".
+00000270: 2020 2020 2020 706f 696e 7465 722d 6576        pointer-ev
+00000280: 656e 7473 3d22 7374 726f 6b65 222f 3e0a  ents="stroke"/>.
+00000290: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+000002a0: 643d 224d 2031 3438 2035 3820 4c20 3338  d="M 148 58 L 38
+000002b0: 2035 3822 0a20 2020 2020 2066 696c 6c3d   58".      fill=
+000002c0: 226e 6f6e 6522 0a20 2020 2020 2073 7472  "none".      str
+000002d0: 6f6b 653d 2223 3530 6661 3762 220a 2020  oke="#50fa7b".  
+000002e0: 2020 2020 7374 726f 6b65 2d77 6964 7468      stroke-width
+000002f0: 3d22 3234 220a 2020 2020 2020 7374 726f  ="24".      stro
+00000300: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
+00000310: 3022 0a20 2020 2020 2070 6f69 6e74 6572  0".      pointer
+00000320: 2d65 7665 6e74 733d 2273 7472 6f6b 6522  -events="stroke"
+00000330: 2f3e 0a20 2020 203c 656c 6c69 7073 650a  />.    <ellipse.
+00000340: 2020 2020 2020 6378 3d22 3938 2e35 220a        cx="98.5".
+00000350: 2020 2020 2020 6379 3d22 3938 2e35 220a        cy="98.5".
+00000360: 2020 2020 2020 7278 3d22 3836 2e35 220a        rx="86.5".
+00000370: 2020 2020 2020 7279 3d22 3836 2e35 220a        ry="86.5".
+00000380: 2020 2020 2020 6669 6c6c 3d22 2330 3030        fill="#000
+00000390: 3022 0a20 2020 2020 2073 7472 6f6b 653d  0".      stroke=
+000003a0: 2223 6262 6265 6337 220a 2020 2020 2020  "#bbbec7".      
+000003b0: 7374 726f 6b65 2d77 6964 7468 3d22 3234  stroke-width="24
+000003c0: 220a 2020 2020 2020 706f 696e 7465 722d  ".      pointer-
+000003d0: 6576 656e 7473 3d22 616c 6c22 2f3e 0a20  events="all"/>. 
+000003e0: 203c 2f67 3e0a 3c2f 7376 673e             </g>.</svg>
```

### Comparing `django-log-lens-0.1.8/django_log_lens/static/django_log_lens/script.js` & `django-log-lens-0.1.9/django_log_lens/static/django_log_lens/script.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,849 +1,850 @@
-"use strict";
-const btnAutoRefresh = document.getElementById("btn-auto-refresh");
-const divLogContent = document.getElementById("div-log-content");
-const divMessageToast = document.getElementById("div-message-toast");
-const divOverlay = document.getElementById("div-overlay");
-const divPrompt = document.getElementById("div-prompt");
-const divToolbar = document.getElementById("div-toolbar");
-const divToolbarExtension = document.getElementById("div-toolbar-extension");
-const h3LogfileName = document.getElementById("h3-logfile-name");
-const inputPathPrefix = /** @type {HTMLInputElement} */ (document.getElementById("input-path-prefix"));
-const inputPathSplitter = /** @type {HTMLInputElement} */ (document.getElementById("input-path-splitter"));
-const inputPrompt = /** @type {HTMLInputElement} */ (document.getElementById("input-prompt"));
-const pMessageToastText = document.getElementById("p-message-toast-text");
-const pPromptText = document.getElementById("p-prompt-text");
-const preLineCounter = document.getElementById("pre-line-counter");
-const preLogContent = document.getElementById("pre-log-content");
-const tableFilePaths = document.getElementById("table-file-paths");
-const tdErrorCountElem = document.getElementById("td-number-of-errors");
-const tdHandlerName = document.getElementById("td-handler-name");
-const tdLineCounter = document.getElementById("td-number-of-lines");
-const tdWarningCount = document.getElementById("td-number-of-warnings");
-
-const HTML_ELEMENTS = [
-    btnAutoRefresh,
-    divLogContent,
-    divMessageToast,
-    divOverlay,
-    divPrompt,
-    divToolbar,
-    divToolbarExtension,
-    h3LogfileName,
-    inputPathPrefix,
-    inputPathSplitter,
-    inputPrompt,
-    pMessageToastText,
-    pPromptText,
-    preLineCounter,
-    preLogContent,
-    tableFilePaths,
-    tdErrorCountElem,
-    tdHandlerName,
-    tdLineCounter,
-    tdWarningCount,
-];
-
-for (let elem of HTML_ELEMENTS) {
-    console.assert(Boolean(elem), `Element not found.`);
-}
-
-const state = {
-    currentError: -1,
-    errorCounter: 0,
-    filePaths: {},
-    lastLogDataTimeStamp: -1,
-    lastSelectedHandlerName: "",
-    timeout: 5000,
-    timeOutId: null,
-    warningCounter: 0,
-};
-
-const preservedState = {
-    autoRefreshState: "off",
-    pathPrefix: "",
-    pathSplitter: "",
-    stringSearchValue: "",
-    stringReplaceValue: "",
-};
-
-let promptCancelCallback = /** @type Function */ ((...args) => {});
-let promptConfirmCallback = /** @type Function */ ((...args) => {});
-
-const _bindings = {
-    propCounter: 0,
-};
-
-/**
- * Binds an element's value to an object's property.
- * @param {HTMLInputElement} elem the HTML element to bind to
- * @param {object} obj the object to bind to
- * @param {string} objProp the name of the property on the object
- * @param {boolean} twoWay whether the binding should be two-way or one-way
- * @param {Function} onChangeCallback the callback function to be called when the property changes
- */
-function bindElementValue(elem, obj, objProp, twoWay = false, onChangeCallback = () => {}) {
-    if (obj[objProp] === undefined) {
-        throw Error("Property '" + objProp + "' does not exist on object.");
-    }
-    const changerHandler = () => {
-        obj[objProp] = elem.value;
-        if (!twoWay) {
-            onChangeCallback(obj, objProp);
-        }
-    };
-    elem.addEventListener("change", changerHandler);
-    if (twoWay) {
-        bindBack(obj, objProp, elem);
-    }
-
-    function bindBack(obj, objProp, elem) {
-        const propId = _bindings.propCounter;
-        _bindings.propCounter++;
-        if (obj[objProp]) {
-            elem.value = obj[objProp];
-            _bindings[`_${propId}`] = obj[objProp];
-        }
-        Object.defineProperty(obj, objProp, {
-            get() {
-                return _bindings[`_${propId}`];
-            },
-            set(value) {
-                _bindings[`_${propId}`] = value;
-                elem.value = value;
-                onChangeCallback(obj, objProp);
-            },
-        });
-    }
-}
-
-/**
- * Binds an element's attribute to an object's property.
- * @param {HTMLElement} elem the HTML element to bind to
- * @param {string} elemAttr the HTML attribute to bind to
- * @param {object} obj object to bind to
- * @param {string} objProp name of the property on the object
- * @param {boolean} twoWay whether the binding should be two-way or one-way
- * @param {Function} onChangeCallback the callback function to be called when the property changes
- */
-function bindElementAttr(elem, elemAttr, obj, objProp, twoWay = false, onChangeCallback = () => {}) {
-    if (obj[objProp] === undefined) {
-        throw Error("Property '" + objProp + "' does not exist on object.");
-    }
-    const handler = () => {
-        obj[objProp] = elem.getAttribute(elemAttr);
-        if (!twoWay) {
-            onChangeCallback(obj, objProp);
-        }
-    };
-    if (elem.tagName === "BUTTON") {
-        elem.addEventListener("click", handler);
-    } else {
-        elem.addEventListener("change", handler);
-    }
-    if (twoWay) {
-        bindAttrBack(obj, objProp, elem, elemAttr, onChangeCallback);
-    }
-}
-
-/**
- * Bind back the object property to the element attribute.
- * @param {object} obj the object to bind to
- * @param {string} objProp the name of the property on the object
- * @param {HTMLElement} elem the HTML element to bind to
- * @param {string} elemAttr the HTML attribute to bind to
- * @param {Function} onChangeCallback the callback function to be called when the property changes
- */
-function bindAttrBack(obj, objProp, elem, elemAttr, onChangeCallback) {
-    const propId = _bindings.propCounter;
-    _bindings.propCounter++;
-    if (obj[objProp]) {
-        elem.setAttribute(elemAttr, obj[objProp]);
-    }
-    _bindings[`_${propId}`] = obj[objProp];
-    Object.defineProperty(obj, objProp, {
-        get() {
-            return _bindings[`_${propId}`];
-        },
-        set(value) {
-            _bindings[`_${propId}`] = value;
-            elem.setAttribute(elemAttr, value);
-            onChangeCallback(obj, objProp);
-        },
-    });
-}
-
-/**
- * Stores the obj[objProp] in the hash so that the page can be restored when refreshed.
- * @param {object} obj the object to be observed
- * @param {string} objProp the property to be stored in the hash
- */
-function bindingObserverFn(obj, objProp) {
-    window.location.hash = encodeURIComponent(btoa(JSON.stringify({
-        preservedState
-    })));
-    console.debug("Changed property:", objProp, ":", obj[objProp]);
-}
-
-/**
- * Sets up the keydown event listeners for the overlay and the window
- * so that the user can confirm or cancel the prompt with the Enter or Escape key.
- * Also sets up the keydown event listener for the window so that the user can refresh the page with F5.
- * @returns {void}
- */
-function setUpEventListeners() {
-    divOverlay.addEventListener("keydown", (event) => {
-        if (event.key === "Enter") {
-            promptOnConfirm();
-        } else if (event.key === "Escape") {
-            promptOnCancel();
-        }
-    });
-
-    window.addEventListener("keydown", (event) => {
-        if (event.key === "F5" && !event.ctrlKey) {
-            event.preventDefault();
-            fetchLogfile();
-        }
-    });
-}
-
-/**
- * Handles the click event of the refresh button.
- * Toggles the state of the button.
- * @param {HTMLElement} btn The invoking button
- */
-function onRefreshBtnClick(btn) {
-    if (btn.getAttribute("state") === "on") {
-        btn.setAttribute("state", "off");
-    } else {
-        btn.setAttribute("state", "on");
-    }
-}
-
-/**
- * Handles the click event of the prompt confirm button.
- * Hides the prompt and calls the confirm callback.
- * @returns {void}
- */
-function promptOnConfirm() {
-    divOverlay.style.display = "none";
-    const input = inputPrompt.value;
-    inputPrompt.value = "";
-    if (promptConfirmCallback) {
-        promptConfirmCallback(input);
-    }
-}
-
-/**
- * Shows a prompt to the user with the given message.
- * @param {string} message the message to be displayed
- * @param {Function} confirmCallback the callback to be called when the user confirms
- * @param {Function} cancelCallback the callback to be called when the user cancels
- */
-function prompt(message, confirmCallback, cancelCallback) {
-    pPromptText.innerText = message;
-    divOverlay.style.display = "block";
-    inputPrompt.focus();
-    promptConfirmCallback = confirmCallback;
-    promptCancelCallback = cancelCallback;
-}
-
-/**
- * Handles the click event of the prompt cancel button.
- * Hides the prompt and calls the cancel callback.
- * @returns {void}
- */
-function promptOnCancel() {
-    divOverlay.style.display = "none";
-    inputPrompt.value = "";
-    if (promptCancelCallback) {
-        promptCancelCallback();
-    }
-}
-
-/**
- * Shows a message toast with the given message and color.
- * Uses a default color if none is provided.
- * @param {string} message
- * @param {string=} color
- */
-function showMessageToast(message, color) {
-    if (color) {
-        divMessageToast.style.color = `var(--${color}`;
-    } else {
-        divMessageToast.style.color = "var(--control-elem-color)";
-    }
-
-    pMessageToastText.innerHTML = message.replaceAll("\n", "<br/>");
-    divMessageToast.style.display = "block";
-    if (state.timeOutId) {
-        clearTimeout(state.timeOutId);
-    }
-    state.timeOutId = setTimeout(() => {
-        divMessageToast.style.display = "none";
-    }, state.timeout);
-}
-
-/**
- * Toggles the visibility of the toolbar extension.
- * Changes the text of the button accordingly.
- * @param {HTMLElement} btn the invoking button
- */
-function toggleToolbarExtensionVisibility(btn) {
-    if (divToolbarExtension.style.display === "none") {
-        divToolbarExtension.style.display = "block";
-        btn.innerText = "Show Less";
-        adjustLogContentMargin();
-    } else {
-        divToolbarExtension.style.display = "none";
-        btn.innerText = "Show More";
-        adjustLogContentMargin();
-    }
-}
-
-/**
- * Fetches the timestamp of the log file to check if it has changed.
- * @param {string=} handlerName
- * @returns {void}
- */
-function requestLogfileTimestamp(handlerName) {
-    handlerName = handlerName || state.lastSelectedHandlerName;
-    if (!handlerName) {
-        return;
-    }
-    // @ts-ignore
-    fetch(requestLogfileTimestampURL + handlerName)
-        .then((response) => response.json())
-        .then((data) => {
-            if (data.timestamp !== state.lastLogDataTimeStamp && state.lastLogDataTimeStamp !== -1) {
-                if (btnAutoRefresh.getAttribute("state") === "on") {
-                    fetchLogfile();
-                } else {
-                    showMessageToast("Logfile has changed.\nClick refresh for an update.", "yellow-color");
-                }
-            }
-        })
-        .catch((error) => {
-            console.error("Error requesting logfile timestamp:", error);
-        });
-}
-
-/**
- * Renders the file path table that displays the handler name and the file path and
- * allows the user to load the log file or clear it.
- * @param {object} data the log config as it is stored in the settings.py
- */
-function renderFilePathTable(data) {
-    for (let prop of Object.keys(data)) {
-        const tr = document.createElement("tr");
-        const tdHandler = document.createElement("td");
-        const tdPath = document.createElement("td");
-        const tdLoad = document.createElement("td");
-        const tdClear = document.createElement("td");
-        tdLoad.innerHTML = "&nbsp;&nbsp;&rarr;&nbsp;&nbsp;";
-        tdLoad.onclick = () => {
-            const tempProp = prop;
-            fetchLogfile(tempProp);
-        };
-        tdLoad.classList.add("clickable");
-        state.lastSelectedHandlerName = prop;
-        tdHandler.innerText = prop;
-        tdPath.innerText = data[prop];
-        tdClear.innerHTML = "&nbsp;&nbsp;&times;&nbsp;&nbsp;";
-        tdClear.classList.add("clickable");
-        tdClear.onclick = () => {
-            const tempProp = prop;
-            promptClearLogFile(tempProp);
-        };
-        tr.appendChild(tdHandler);
-        tr.appendChild(tdPath);
-        tr.appendChild(tdLoad);
-        tr.appendChild(tdClear);
-        const rows = tableFilePaths.getElementsByTagName("tr");
-        for (let i = 1; i < rows.length; i++) {
-            if (rows[i].getElementsByTagName("td")[0].innerText === prop) {
-                tableFilePaths.removeChild(rows[i]);
-            }
-        }
-        tableFilePaths.appendChild(tr);
-    }
-}
-
-/**
- * Fetches the CSRF token from the input elements of the page.
- * See https://gist.github.com/sirodoht/fb7a6e98d33fc460d4f1eadaff486e7b - thanks!
- * @returns {string} - the CSRF token
- */
-function getCsrf() {
-    const inputElements = document.querySelectorAll("input");
-    let csrfToken = "";
-    for (let i = 0; i < inputElements.length; ++i) {
-        if (inputElements[i].name === "csrfmiddlewaretoken") {
-            csrfToken = inputElements[i].value;
-            break;
-        }
-    }
-    return csrfToken;
-}
-
-/**
- * Fetches the file paths to the log files from the server.
- * In case no file paths are found, a message is displayed to the user
- * that they need to set up a logging configuration in their settings.py.
- * @returns {void}
- */
-function fetchFilePaths() {
-    showMessageToast("Fetching file paths...");
-
-    // @ts-ignore
-    fetch(requestLogFilePathsURL)
-        .then((response) => response.json())
-        .then((data) => {
-            state.filePaths = data;
-            if (Object.keys(data).length === 0) {
-                showMessageToast(
-                    "You need to set up a LOGGING configuration\n in your settings.py\n in order to manage your logs here.",
-                    "light-red-color"
-                );
-                tableFilePaths.style.display = "none";
-                return;
-            } else {
-                tableFilePaths.style.display = "";
-                renderFilePathTable(data);
-                showMessageToast("Fetched file paths.", "green-color");
-            }
-        })
-        .catch((error) => {
-            showMessageToast("Error fetching file paths.", "light-red-color");
-            console.error("Error fetching file paths:", error);
-        });
-}
-
-/**
- * Shows a prompt to the user to confirm if they want to clear the log file.
- * @param {string} handlerName
- * @returns {void}
- */
-function promptClearLogFile(handlerName) {
-    const callbackCanceled = () => showMessageToast("Did NOT clear logfile.", "light-red-color");
-    const callbackConfirmed = (promptText) => {
-        if (promptText === handlerName) {
-            clearLogFile(handlerName);
-        } else callbackCanceled();
-    };
-    const promptText =
-        `Are you sure you want to clear the logs of ${handlerName}?\n` + `If so, type ${handlerName} in the field below.`;
-    prompt(promptText, callbackConfirmed, callbackCanceled);
-}
-
-/**
- * Clears the log file of the given handler name.
- * @param {string} handlerName
- * @returns {void}
- */
-function clearLogFile(handlerName) {
-    if (!handlerName) {
-        return;
-    }
-    // @ts-ignore
-    fetch(clearLogFileURL + handlerName, {
-            method: "DELETE",
-            headers: {
-                "X-CSRFToken": getCsrf()
-            },
-        })
-        .then((response) => {
-            if (response.status >= 400) {
-                handleFetchLogFileError(response);
-            }
-            return response.text(); // todo simplify the chain
-        })
-        .then(() => {
-            fetchLogfile();
-            showMessageToast("Cleared logfile of '" + handlerName + "'.", "green-color");
-        })
-        .catch((error) => {
-            showMessageToast("Error clearing file.", "light-red-color");
-            console.error("Error clearing file:", error);
-        });
-}
-
-/**
- * Adjusts the margin of the log content to make space for the toolbar.
- * @returns {void}
- */
-function adjustLogContentMargin() {
-    divLogContent.style.marginTop = getOffset() + "px";
-}
-
-/**
- * Handles the error when fetching the log file.
- * Displays the error message to the user.
- * Updates the log content with the error message.
- * @param {Response} response
- */
-function handleFetchLogFileError(response) {
-    response.text().then((text) => {
-        adjustLogContentMargin();
-        preLogContent.innerText = text;
-    });
-    throw Error("Error fetching log file.");
-}
-
-/**
- * Fetches the log file of the given handler name.
- * If no handler name is provided, the last selected handler name is used.
- * If no handler name is available, a message is displayed to the user.
- * @param {string=} handlerName
- * @returns {void}
- */
-function fetchLogfile(handlerName) {
-    showMessageToast("Fetching log file...");
-    if (!handlerName) {
-        handlerName = state.lastSelectedHandlerName;
-        if (!handlerName) {
-            showMessageToast("No handler selected.", "light-red-color");
-            return;
-        }
-    }
-    // @ts-ignore
-    fetch(requestLogfileURL + handlerName)
-        .then((response) => {
-            if (response.status >= 400) {
-                handleFetchLogFileError(response);
-            }
-            return response.json();
-        })
-        .then((jsonResponse) => {
-            let logText = jsonResponse.text;
-            if (jsonResponse.timestamp === state.lastLogDataTimeStamp && handlerName === state.lastSelectedHandlerName) {
-                showMessageToast("Logfile has not changed.", "cyan-color");
-                return null;
-            }
-
-            state.lastLogDataTimeStamp = jsonResponse.timestamp;
-            state.lastSelectedHandlerName = handlerName;
-            tdHandlerName.innerText = handlerName;
-
-            adjustLogContentMargin();
-            checkLogFileLength(logText);
-            showMessageToast("Fetched log file.", "green-color");
-
-            setTimeout(() => {
-                finalize(logText, handlerName);
-            }, 250); // set timeout to allow the toast to be displayed
-        })
-        .catch((error) => {
-            showMessageToast(error.message || "Error fetching log file.", "light-red-color");
-            console.error("Error fetching log file:", error);
-        });
-}
-
-/**
- * Finalizes the log text after fetching the log file.
- * - Renders the log text
- * - Updates the line counter
- * - Updates the error and warning counter
- * - Updates the log file name
- * - Scrolls to the bottom of the page
- * @param {string} logText
- * @param {string} handlerName
- * @returns {void}
- */
-function finalize(logText, handlerName) {
-    const logLines = logText.split("\n");
-    preLogContent.innerHTML = renderLogText(logLines);
-    tdLineCounter.innerText = String(logLines.length);
-    tdErrorCountElem.innerText = String(state.errorCounter);
-    tdWarningCount.innerText = String(state.warningCounter);
-    h3LogfileName.innerText = state.filePaths[handlerName];
-    addLineNumbers(logLines.length);
-    window.scrollTo(0, document.body.scrollHeight);
-}
-
-/**
- * Adds line numbers to the line counter.
- * @param {number} noOfLines
- */
-function addLineNumbers(noOfLines) {
-    preLineCounter.innerHTML = "";
-    const lineCounterLines = [];
-    for (let i = 0; i < noOfLines; i++) {
-        lineCounterLines[i] = `<span id='line-${i + 1}' class='line-counter'>`.concat(
-            (i + 1).toString().padStart(5, "0"),
-            "</span><br />"
-        );
-    }
-    preLineCounter.innerHTML = lineCounterLines.join("");
-}
-
-/**
- * Checks if the log file is too large to render.
- * If it is, the log content is cleared and an error is thrown.
- * @param {string} logText the log text to be checked
- * @returns {void}
- */
-function checkLogFileLength(logText) {
-    const lineCounter = logText.split("\n").length;
-    if (lineCounter > 25000) {
-        preLogContent.innerHTML = "";
-        tdErrorCountElem.innerText = "?";
-        tdWarningCount.innerText = "?";
-        tdLineCounter.innerText = String(lineCounter);
-        throw Error("Logfile is too large to render.");
-    }
-}
-
-function renderLine(line, lineCounter) {
-    const matchesStringRegex = line.match(/"([^"]+)"/g);
-    const matchesLineNumberRegex = line.match(/, line \b\d+\b,/g);
-    const containsUrlRegex = /\bhttps?:\/\/[^/]+(\/[^/]+)\b/;
-
-    if (matchesStringRegex && matchesLineNumberRegex) {
-        const lineNumber = matchesLineNumberRegex[matchesLineNumberRegex.length - 1]
-            .replace(/, line /g, "")
-            .replace(/,/g, "");
-        let filename = matchesStringRegex[matchesStringRegex.length - 1].replace(/"/g, "");
-        line = line.replace(
-            /"([^"]+)"/g,
-            `"<span class="quoted-text" line_number=${lineNumber} onclick="copyElementToClipboard(this)">$1</span>"`
-        );
-        line += ` <a  id="a-${lineCounter}" href="javascript:openInVsCode(document.getElementById(\`a-${lineCounter}\`))"
-                        title="open in VS Code"
-                        file_name="${filename}"
-                        line_number="${lineNumber}"> &uarr; </a>`;
-    } else if (matchesStringRegex) {
-        line = line.replace(/"([^"]+)"/g, '"<span class="quoted-text" onclick="copyElementToClipboard(this)">$1</span>"');
-    } else if (containsUrlRegex.test(line)) {
-        const urlRegex = /\bhttps?:\/\/[^/]+(\/[^/]+)*\b(?=\))/g;
-        const url = line.match(urlRegex) ? line.match(urlRegex)[0] : null;
-        line = line.replace(urlRegex, `<span class="url" onclick="copyElementToClipboard(this)">$&</span>`);
-        if (url) {
-            line += ` <a  id="a-${lineCounter}" href="javascript:openInVsCode(document.getElementById(\`a-${lineCounter}\`))"
-                        title="open in VS Code"
-                        file_name="${url}"> &uarr; </a>`;
-        }
-    }
-
-    line = line.replace(/'([^']+)'/g, `'<span class="quoted-text" onclick="copyElementToClipboard(this)">$1</span>'`);
-    return line;
-}
-
-/**
- * Colors the log lines based on the log level that
- * are extracted from the [LVL:XX] prefix.
- * @param {string} line
- * @returns
- */
-function colorLogLevels(line) {
-    const prefixPattern = /\[LVL:(\d+)\]/;
-    const prefixMatch = line.match(prefixPattern);
-    if (prefixMatch) {
-        const fullMatch = prefixMatch[0];
-        const logLevel = parseInt(prefixMatch[1]);
-        if (logLevel >= 50) {
-            line = line.replace(fullMatch, `</span><span id="error-${state.errorCounter}" class="critical">`);
-            state.errorCounter++;
-        } else if (logLevel >= 40) {
-            line = line.replace(fullMatch, `</span><span id="error-${state.errorCounter}" class="error">`);
-            state.errorCounter++;
-        } else if (logLevel >= 30) {
-            line = line.replace(fullMatch, `</span><span class="warning">`);
-            state.warningCounter++;
-        } else if (logLevel >= 20) {
-            line = line.replace(fullMatch, `</span><span class="info">`);
-        } else {
-            line = line.replace(fullMatch, `</span><span class="debug">`);
-        }
-    }
-    return line;
-}
-
-/**
- * Renders the log text - highlights errors, warnings, and info messages.
- * Adds line numbers to the log text.
- * @param {string[]} logLines - the log text to be rendered
- * @returns {string} - the formatted log text as HTML
- */
-function renderLogText(logLines) {
-    let formattedLog = "";
-    let lineCounter = 1;
-
-    state.currentError = -1;
-    state.errorCounter = 0;
-    state.warningCounter = 0;
-
-    for (let i = 0; i < logLines.length; i++) {
-        logLines[i] = renderLine(logLines[i], lineCounter) + "<br />";
-        logLines[i] = colorLogLevels(logLines[i]);
-        lineCounter++;
-    }
-    formattedLog = logLines.join("");
-    return `<span>${formattedLog}</span>`;
-}
-
-/**
- * Returns the offset of the toolbar.
- * @returns {number}
- */
-function getOffset() {
-    return divToolbar.offsetHeight - 1;
-}
-
-/**
- * Opens the file in VS Code.
- * The invoking element must have the attributes file_name and line_number.
- * @param {HTMLElement} element - the invoking element
- * @returns {void}
- */
-function openInVsCode(element) {
-    let fileName = element.getAttribute("file_name");
-    const lineNumber = element.getAttribute("line_number");
-    fileName = splitPath(fileName);
-    fileName = preservedState.stringSearchValue ?
-        fileName.replace(preservedState.stringSearchValue, preservedState.stringReplaceValue) :
-        fileName;
-    const url = lineNumber ? `vscode://file/${fileName}:${lineNumber}` : `vscode://file/${fileName}`;
-    window.open(url);
-}
-
-/**
- * Splits the path at the splitter and returns the last part.
- * @param {string} path
- * @returns {string} - the last part of the path
- */
-function splitPath(path) {
-    const prefix = inputPathPrefix.value;
-    const splitter = inputPathSplitter.value;
-    const splitted = path.split(splitter);
-    if (!splitter) {
-        return path;
-    } else if (splitted.length > 1) {
-        return prefix + splitted[splitted.length - 1];
-    }
-    return splitted[splitted.length - 1];
-}
-
-/**
- * Copies the text of the invoking element to the clipboard.
- * If the element has a line_number attribute, it is appended to the text.
- * @param {HTMLElement} HTMLElement - the invoking element
- * @returns {void}
- */
-function copyElementToClipboard(HTMLElement) {
-    const text = HTMLElement.innerText;
-    const tempInput = document.createElement("input");
-    tempInput.value = text;
-    if (inputPathSplitter) {
-        tempInput.value = splitPath(text);
-    }
-    document.body.appendChild(tempInput);
-    if (HTMLElement.hasAttribute("line_number")) {
-        tempInput.value += ":" + HTMLElement.getAttribute("line_number");
-    }
-    tempInput.select();
-    document.execCommand("copy");
-    showMessageToast(`${tempInput.value}<br/><span class="info">Copied to clipboard!</span>`);
-    document.body.removeChild(tempInput);
-}
-
-/**
- * Scrolls to the line with the given id.
- * @param {string} id
- * @returns {void}
- */
-function goToLineWidId(id) {
-    const scrollOffset = getOffset();
-    try {
-        const _id = parseInt(id);
-        const line = document.getElementById("line-" + _id);
-        line.scrollIntoView();
-        window.scroll(0, window.scrollY - scrollOffset);
-    } catch {}
-}
-
-/**
- * Scrolls start of the error with the given error number.
- * @param {number} errorNo
- * @returns {void}
- */
-function goToError(errorNo) {
-    const scrollOffset = getOffset();
-    const errorElement = document.getElementById(`error-${errorNo}`);
-    const errYPos = errorElement.getBoundingClientRect().top;
-
-    if (errYPos + window.scrollY - document.body.scrollHeight > 0) {
-        window.scroll(0, document.body.scrollHeight);
-    } else {
-        errorElement.scrollIntoView();
-        window.scroll(0, window.scrollY - scrollOffset);
-    }
-
-    errorElement.style.backgroundColor = "var(--highlight-color)";
-    setTimeout(() => {
-        errorElement.style.backgroundColor = "";
-    }, state.timeout);
-}
-
-/**
- * Scrolls to the latest error.
- * @returns {void}
- */
-function goToLastError() {
-    if (state.errorCounter > 0) {
-        state.currentError = state.errorCounter - 1;
-        goToError(state.currentError);
-    }
-}
-
-/**
- * Scrolls to the next error in the log file.
- * @returns {void}
- */
-function goToNextError() {
-    if (state.currentError < state.errorCounter - 1) {
-        state.currentError++;
-        goToError(state.currentError);
-    }
-}
-
-/**
- * Scrolls to the previous error in the log file.
- * @returns {void}
- */
-function goToPreviousError() {
-    if (state.currentError > 0) {
-        state.currentError--;
-        goToError(state.currentError);
-    }
-}
-
-/**
- * Sets up the page:
- * - Parses the hash so that the page can be restored to its previous state
- * - Sets up event listeners
- * - Fetches file paths from the server
- * - Requests the timestamp of the log file so that the user can be notified if the log file has changed
- */
-function setUpPage() {
-    try {
-        const hash = decodeURIComponent(window.location.hash.substring(1));
-        Object.assign(preservedState, JSON.parse(atob(hash)).preservedState);
-    } catch (error) {
-        console.debug("Did not parse hash:", error);
-    }
-
-    bindElementValue(inputPathPrefix, preservedState, "pathPrefix", true, bindingObserverFn);
-    bindElementValue(inputPathSplitter, preservedState, "pathSplitter", true, bindingObserverFn);
-    bindElementAttr(btnAutoRefresh, "state", preservedState, "autoRefreshState", true, bindingObserverFn);
-    window.onload = () => {
-        setUpEventListeners();
-        fetchFilePaths();
-        setInterval(() => {
-            requestLogfileTimestamp();
-        }, 2 * state.timeout);
-    };
-    adjustLogContentMargin();
-}
-
+"use strict";
+const btnAutoRefresh = document.getElementById("btn-auto-refresh");
+const divLogContent = document.getElementById("div-log-content");
+const divMessageToast = document.getElementById("div-message-toast");
+const divOverlay = document.getElementById("div-overlay");
+const divPrompt = document.getElementById("div-prompt");
+const divToolbar = document.getElementById("div-toolbar");
+const divToolbarExtension = document.getElementById("div-toolbar-extension");
+const h3LogfileName = document.getElementById("h3-logfile-name");
+const inputPathPrefix = /** @type {HTMLInputElement} */ (document.getElementById("input-path-prefix"));
+const inputPathSplitter = /** @type {HTMLInputElement} */ (document.getElementById("input-path-splitter"));
+const inputPrompt = /** @type {HTMLInputElement} */ (document.getElementById("input-prompt"));
+const pMessageToastText = document.getElementById("p-message-toast-text");
+const pPromptText = document.getElementById("p-prompt-text");
+const preLineCounter = document.getElementById("pre-line-counter");
+const preLogContent = document.getElementById("pre-log-content");
+const tableFilePaths = document.getElementById("table-file-paths");
+const tdErrorCountElem = document.getElementById("td-number-of-errors");
+const tdHandlerName = document.getElementById("td-handler-name");
+const tdLineCounter = document.getElementById("td-number-of-lines");
+const tdWarningCount = document.getElementById("td-number-of-warnings");
+
+const HTML_ELEMENTS = [
+    btnAutoRefresh,
+    divLogContent,
+    divMessageToast,
+    divOverlay,
+    divPrompt,
+    divToolbar,
+    divToolbarExtension,
+    h3LogfileName,
+    inputPathPrefix,
+    inputPathSplitter,
+    inputPrompt,
+    pMessageToastText,
+    pPromptText,
+    preLineCounter,
+    preLogContent,
+    tableFilePaths,
+    tdErrorCountElem,
+    tdHandlerName,
+    tdLineCounter,
+    tdWarningCount,
+];
+
+for (let elem of HTML_ELEMENTS) {
+    console.assert(Boolean(elem), `Element not found.`);
+}
+
+const state = {
+    currentError: -1,
+    errorCounter: 0,
+    filePaths: {},
+    lastLogDataTimeStamp: -1,
+    lastSelectedHandlerName: "",
+    timeout: 5000,
+    timeOutId: null,
+    warningCounter: 0,
+};
+
+const preservedState = {
+    autoRefreshState: "off",
+    pathPrefix: "",
+    pathSplitter: "",
+    stringSearchValue: "",
+    stringReplaceValue: "",
+};
+
+let promptCancelCallback = /** @type Function */ ((...args) => {});
+let promptConfirmCallback = /** @type Function */ ((...args) => {});
+
+const _bindings = {
+    propCounter: 0,
+};
+
+/**
+ * Binds an element's value to an object's property.
+ * @param {HTMLInputElement} elem the HTML element to bind to
+ * @param {object} obj the object to bind to
+ * @param {string} objProp the name of the property on the object
+ * @param {boolean} twoWay whether the binding should be two-way or one-way
+ * @param {Function} onChangeCallback the callback function to be called when the property changes
+ */
+function bindElementValue(elem, obj, objProp, twoWay = false, onChangeCallback = () => {}) {
+    if (obj[objProp] === undefined) {
+        throw Error("Property '" + objProp + "' does not exist on object.");
+    }
+    const changerHandler = () => {
+        obj[objProp] = elem.value;
+        if (!twoWay) {
+            onChangeCallback(obj, objProp);
+        }
+    };
+    elem.addEventListener("change", changerHandler);
+    if (twoWay) {
+        bindBack(obj, objProp, elem);
+    }
+
+    function bindBack(obj, objProp, elem) {
+        const propId = _bindings.propCounter;
+        _bindings.propCounter++;
+        if (obj[objProp]) {
+            elem.value = obj[objProp];
+            _bindings[`_${propId}`] = obj[objProp];
+        }
+        Object.defineProperty(obj, objProp, {
+            get() {
+                return _bindings[`_${propId}`];
+            },
+            set(value) {
+                _bindings[`_${propId}`] = value;
+                elem.value = value;
+                onChangeCallback(obj, objProp);
+            },
+        });
+    }
+}
+
+/**
+ * Binds an element's attribute to an object's property.
+ * @param {HTMLElement} elem the HTML element to bind to
+ * @param {string} elemAttr the HTML attribute to bind to
+ * @param {object} obj object to bind to
+ * @param {string} objProp name of the property on the object
+ * @param {boolean} twoWay whether the binding should be two-way or one-way
+ * @param {Function} onChangeCallback the callback function to be called when the property changes
+ */
+function bindElementAttr(elem, elemAttr, obj, objProp, twoWay = false, onChangeCallback = () => {}) {
+    if (obj[objProp] === undefined) {
+        throw Error("Property '" + objProp + "' does not exist on object.");
+    }
+    const handler = () => {
+        obj[objProp] = elem.getAttribute(elemAttr);
+        if (!twoWay) {
+            onChangeCallback(obj, objProp);
+        }
+    };
+    if (elem.tagName === "BUTTON") {
+        elem.addEventListener("click", handler);
+    } else {
+        elem.addEventListener("change", handler);
+    }
+    if (twoWay) {
+        bindAttrBack(obj, objProp, elem, elemAttr, onChangeCallback);
+    }
+}
+
+/**
+ * Bind back the object property to the element attribute.
+ * @param {object} obj the object to bind to
+ * @param {string} objProp the name of the property on the object
+ * @param {HTMLElement} elem the HTML element to bind to
+ * @param {string} elemAttr the HTML attribute to bind to
+ * @param {Function} onChangeCallback the callback function to be called when the property changes
+ */
+function bindAttrBack(obj, objProp, elem, elemAttr, onChangeCallback) {
+    const propId = _bindings.propCounter;
+    _bindings.propCounter++;
+    if (obj[objProp]) {
+        elem.setAttribute(elemAttr, obj[objProp]);
+    }
+    _bindings[`_${propId}`] = obj[objProp];
+    Object.defineProperty(obj, objProp, {
+        get() {
+            return _bindings[`_${propId}`];
+        },
+        set(value) {
+            _bindings[`_${propId}`] = value;
+            elem.setAttribute(elemAttr, value);
+            onChangeCallback(obj, objProp);
+        },
+    });
+}
+
+/**
+ * Stores the obj[objProp] in the hash so that the page can be restored when refreshed.
+ * @param {object} obj the object to be observed
+ * @param {string} objProp the property to be stored in the hash
+ */
+function bindingObserverFn(obj, objProp) {
+    window.location.hash = encodeURIComponent(btoa(JSON.stringify({
+        preservedState
+    })));
+    console.debug("Changed property:", objProp, ":", obj[objProp]);
+}
+
+/**
+ * Sets up the keydown event listeners for the overlay and the window
+ * so that the user can confirm or cancel the prompt with the Enter or Escape key.
+ * Also sets up the keydown event listener for the window so that the user can refresh the page with F5.
+ * @returns {void}
+ */
+function setUpEventListeners() {
+    divOverlay.addEventListener("keydown", (event) => {
+        if (event.key === "Enter") {
+            promptOnConfirm();
+        } else if (event.key === "Escape") {
+            promptOnCancel();
+        }
+    });
+
+    window.addEventListener("keydown", (event) => {
+        if (event.key === "F5" && !event.ctrlKey) {
+            event.preventDefault();
+            fetchLogfile();
+        }
+    });
+}
+
+/**
+ * Handles the click event of the refresh button.
+ * Toggles the state of the button.
+ * @param {HTMLElement} btn The invoking button
+ */
+function onRefreshBtnClick(btn) {
+    if (btn.getAttribute("state") === "on") {
+        btn.setAttribute("state", "off");
+    } else {
+        btn.setAttribute("state", "on");
+    }
+}
+
+/**
+ * Handles the click event of the prompt confirm button.
+ * Hides the prompt and calls the confirm callback.
+ * @returns {void}
+ */
+function promptOnConfirm() {
+    divOverlay.style.display = "none";
+    const input = inputPrompt.value;
+    inputPrompt.value = "";
+    if (promptConfirmCallback) {
+        promptConfirmCallback(input);
+    }
+}
+
+/**
+ * Shows a prompt to the user with the given message.
+ * @param {string} message the message to be displayed
+ * @param {Function} confirmCallback the callback to be called when the user confirms
+ * @param {Function} cancelCallback the callback to be called when the user cancels
+ */
+function prompt(message, confirmCallback, cancelCallback) {
+    pPromptText.innerText = message;
+    divOverlay.style.display = "block";
+    inputPrompt.focus();
+    promptConfirmCallback = confirmCallback;
+    promptCancelCallback = cancelCallback;
+}
+
+/**
+ * Handles the click event of the prompt cancel button.
+ * Hides the prompt and calls the cancel callback.
+ * @returns {void}
+ */
+function promptOnCancel() {
+    divOverlay.style.display = "none";
+    inputPrompt.value = "";
+    if (promptCancelCallback) {
+        promptCancelCallback();
+    }
+}
+
+/**
+ * Shows a message toast with the given message and color.
+ * Uses a default color if none is provided.
+ * @param {string} message
+ * @param {string=} color
+ */
+function showMessageToast(message, color) {
+    if (color) {
+        divMessageToast.style.color = `var(--${color}`;
+    } else {
+        divMessageToast.style.color = "var(--control-elem-color)";
+    }
+
+    pMessageToastText.innerHTML = message.replaceAll("\n", "<br/>");
+    divMessageToast.style.display = "flex";
+    if (state.timeOutId) {
+        clearTimeout(state.timeOutId);
+    }
+    state.timeOutId = setTimeout(() => {
+        divMessageToast.style.display = "none";
+    }, state.timeout);
+}
+
+/**
+ * Toggles the visibility of the toolbar extension.
+ * Changes the text of the button accordingly.
+ * @param {HTMLElement} btn the invoking button
+ */
+function toggleToolbarExtensionVisibility(btn) {
+    if (divToolbarExtension.style.display === "none") {
+        divToolbarExtension.style.display = "block";
+        btn.innerText = "Show Less";
+        adjustLogContentMargin();
+    } else {
+        divToolbarExtension.style.display = "none";
+        btn.innerText = "Show More";
+        adjustLogContentMargin();
+    }
+}
+
+/**
+ * Fetches the timestamp of the log file to check if it has changed.
+ * @param {string=} handlerName
+ * @returns {void}
+ */
+function requestLogfileTimestamp(handlerName) {
+    handlerName = handlerName || state.lastSelectedHandlerName;
+    if (!handlerName) {
+        return;
+    }
+    // @ts-ignore
+    fetch(requestLogfileTimestampURL + handlerName)
+        .then((response) => response.json())
+        .then((data) => {
+            if (data.timestamp !== state.lastLogDataTimeStamp && state.lastLogDataTimeStamp !== -1) {
+                if (btnAutoRefresh.getAttribute("state") === "on") {
+                    fetchLogfile();
+                } else {
+                    showMessageToast("Logfile has been changed\nClick refresh for an update", "yellow-color");
+                }
+            }
+        })
+        .catch((error) => {
+            console.error("Error requesting logfile timestamp:", error);
+        });
+}
+
+/**
+ * Renders the file path table that displays the handler name and the file path and
+ * allows the user to load the log file or clear it.
+ * @param {object} data the log config as it is stored in the settings.py
+ */
+function renderFilePathTable(data) {
+    for (let prop of Object.keys(data)) {
+        const tr = document.createElement("tr");
+        const tdHandler = document.createElement("td");
+        const tdPath = document.createElement("td");
+        const tdLoad = document.createElement("td");
+        const tdClear = document.createElement("td");
+        tdLoad.innerHTML = "&nbsp;&nbsp;&rarr;&nbsp;&nbsp;";
+        tdLoad.onclick = () => {
+            const tempProp = prop;
+            fetchLogfile(tempProp);
+        };
+        tdLoad.classList.add("clickable");
+        state.lastSelectedHandlerName = prop;
+        tdHandler.innerText = prop;
+        tdPath.innerText = data[prop];
+        tdClear.innerHTML = "&nbsp;&nbsp;&times;&nbsp;&nbsp;";
+        tdClear.classList.add("clickable");
+        tdClear.onclick = () => {
+            const tempProp = prop;
+            promptClearLogFile(tempProp);
+        };
+        tr.appendChild(tdHandler);
+        tr.appendChild(tdPath);
+        tr.appendChild(tdLoad);
+        tr.appendChild(tdClear);
+        const rows = tableFilePaths.getElementsByTagName("tr");
+        for (let i = 1; i < rows.length; i++) {
+            if (rows[i].getElementsByTagName("td")[0].innerText === prop) {
+                tableFilePaths.removeChild(rows[i]);
+            }
+        }
+        tableFilePaths.appendChild(tr);
+    }
+}
+
+/**
+ * Fetches the CSRF token from the input elements of the page.
+ * See https://gist.github.com/sirodoht/fb7a6e98d33fc460d4f1eadaff486e7b - thanks!
+ * @returns {string} - the CSRF token
+ */
+function getCsrf() {
+    const inputElements = document.querySelectorAll("input");
+    let csrfToken = "";
+    for (let i = 0; i < inputElements.length; ++i) {
+        if (inputElements[i].name === "csrfmiddlewaretoken") {
+            csrfToken = inputElements[i].value;
+            break;
+        }
+    }
+    return csrfToken;
+}
+
+/**
+ * Fetches the file paths to the log files from the server.
+ * In case no file paths are found, a message is displayed to the user
+ * that they need to set up a logging configuration in their settings.py.
+ * @returns {void}
+ */
+function fetchFilePaths() {
+    showMessageToast("Fetching file paths...");
+
+    // @ts-ignore
+    fetch(requestLogFilePathsURL)
+        .then((response) => response.json())
+        .then((data) => {
+            state.filePaths = data;
+            if (Object.keys(data).length === 0) {
+                showMessageToast(
+                    "You need to set up a LOGGING configuration\n in your settings.py\n in order to manage your logs here",
+                    "light-red-color"
+                );
+                tableFilePaths.style.display = "none";
+                return;
+            } else {
+                tableFilePaths.style.display = "";
+                renderFilePathTable(data);
+                showMessageToast("Fetched file paths", "green-color");
+            }
+        })
+        .catch((error) => {
+            showMessageToast("Error fetching file paths", "light-red-color");
+            console.error("Error fetching file paths:", error);
+        });
+}
+
+/**
+ * Shows a prompt to the user to confirm if they want to clear the log file.
+ * @param {string} handlerName
+ * @returns {void}
+ */
+function promptClearLogFile(handlerName) {
+    const callbackCanceled = () => showMessageToast("Did NOT clear logfile", "light-red-color");
+    const callbackConfirmed = (promptText) => {
+        if (promptText === handlerName) {
+            clearLogFile(handlerName);
+        } else callbackCanceled();
+    };
+    const promptText =
+        `Are you sure you want to clear the logs of ${handlerName}?\n` + `If so, type ${handlerName} in the field below.`;
+    prompt(promptText, callbackConfirmed, callbackCanceled);
+}
+
+/**
+ * Clears the log file of the given handler name.
+ * @param {string} handlerName
+ * @returns {void}
+ */
+function clearLogFile(handlerName) {
+    if (!handlerName) {
+        return;
+    }
+    // @ts-ignore
+    fetch(clearLogFileURL + handlerName, {
+            method: "DELETE",
+            headers: {
+                "X-CSRFToken": getCsrf()
+            },
+        })
+        .then((response) => {
+            if (response.status >= 400) {
+                handleFetchLogFileError(response);
+            }
+            return response.text(); // todo simplify the chain
+        })
+        .then(() => {
+            fetchLogfile();
+            showMessageToast(`Cleared logfile of '${handlerName}'`, "green-color");
+        })
+        .catch((error) => {
+            showMessageToast("Error clearing file", "light-red-color");
+            console.error("Error clearing file:", error);
+        });
+}
+
+/**
+ * Adjusts the margin of the log content to make space for the toolbar.
+ * @returns {void}
+ */
+function adjustLogContentMargin() {
+    divLogContent.style.marginTop = getOffset() + "px";
+}
+
+/**
+ * Handles the error when fetching the log file.
+ * Displays the error message to the user.
+ * Updates the log content with the error message.
+ * @param {Response} response
+ */
+function handleFetchLogFileError(response) {
+    response.text().then((text) => {
+        adjustLogContentMargin();
+        preLogContent.innerText = text;
+    });
+    throw Error("Error fetching log file");
+}
+
+/**
+ * Fetches the log file of the given handler name.
+ * If no handler name is provided, the last selected handler name is used.
+ * If no handler name is available, a message is displayed to the user.
+ * @param {string=} handlerName
+ * @returns {void}
+ */
+function fetchLogfile(handlerName) {
+    showMessageToast("Fetching log file...");
+    if (!handlerName) {
+        handlerName = state.lastSelectedHandlerName;
+        if (!handlerName) {
+            showMessageToast("No handler selected", "light-red-color");
+            return;
+        }
+    }
+    // @ts-ignore
+    fetch(requestLogfileURL + handlerName)
+        .then((response) => {
+            if (response.status >= 400) {
+                handleFetchLogFileError(response);
+            }
+            return response.json();
+        })
+        .then((jsonResponse) => {
+            let logText = jsonResponse.text;
+            if (jsonResponse.timestamp === state.lastLogDataTimeStamp && handlerName === state.lastSelectedHandlerName) {
+                showMessageToast("No changes detected", "cyan-color");
+                return null;
+            }
+
+            state.lastLogDataTimeStamp = jsonResponse.timestamp;
+            state.lastSelectedHandlerName = handlerName;
+            tdHandlerName.innerText = handlerName;
+
+            adjustLogContentMargin();
+            checkLogFileLength(logText);
+            showMessageToast("Fetched log file", "green-color");
+
+            setTimeout(() => {
+                finalize(logText, handlerName);
+            }, 250); // set timeout to allow the toast to be displayed
+        })
+        .catch((error) => {
+            showMessageToast(error.message || "Error fetching log file", "light-red-color");
+            console.error("Error fetching log file:", error);
+        });
+}
+
+/**
+ * Finalizes the log text after fetching the log file.
+ * - Renders the log text
+ * - Updates the line counter
+ * - Updates the error and warning counter
+ * - Updates the log file name
+ * - Scrolls to the bottom of the page
+ * @param {string} logText
+ * @param {string} handlerName
+ * @returns {void}
+ */
+function finalize(logText, handlerName) {
+    const logLines = logText.split("\n");
+    preLogContent.innerHTML = renderLogText(logLines);
+    tdLineCounter.innerText = String(logLines.length);
+    tdErrorCountElem.innerText = String(state.errorCounter);
+    tdWarningCount.innerText = String(state.warningCounter);
+    h3LogfileName.innerText = state.filePaths[handlerName];
+    addLineNumbers(logLines.length);
+    window.scrollTo(0, document.body.scrollHeight);
+}
+
+/**
+ * Adds line numbers to the line counter.
+ * @param {number} noOfLines
+ */
+function addLineNumbers(noOfLines) {
+    preLineCounter.innerHTML = "";
+    const lineCounterLines = [];
+    for (let i = 0; i < noOfLines; i++) {
+        lineCounterLines[i] = `<span id='line-${i + 1}' class='line-counter'>`.concat(
+            (i + 1).toString().padStart(5, "0"),
+            "</span><br />"
+        );
+    }
+    preLineCounter.innerHTML = lineCounterLines.join("");
+}
+
+/**
+ * Checks if the log file is too large to render.
+ * If it is, the log content is cleared and an error is thrown.
+ * @param {string} logText the log text to be checked
+ * @returns {void}
+ */
+function checkLogFileLength(logText) {
+    const lineCounter = logText.split("\n").length;
+    if (lineCounter > 99999) {
+        preLineCounter.innerHTML = "";
+        preLogContent.innerHTML = "";
+        tdErrorCountElem.innerText = "?";
+        tdWarningCount.innerText = "?";
+        tdLineCounter.innerText = String(lineCounter);
+        throw Error("Logfile is too large to render");
+    }
+}
+
+function renderLine(line, lineCounter) {
+    const matchesStringRegex = line.match(/"([^"]+)"/g);
+    const matchesLineNumberRegex = line.match(/, line \b\d+\b,/g);
+    const containsUrlRegex = /\bhttps?:\/\/[^/]+(\/[^/]+)\b/;
+
+    if (matchesStringRegex && matchesLineNumberRegex) {
+        const lineNumber = matchesLineNumberRegex[matchesLineNumberRegex.length - 1]
+            .replace(/, line /g, "")
+            .replace(/,/g, "");
+        let filename = matchesStringRegex[matchesStringRegex.length - 1].replace(/"/g, "");
+        line = line.replace(
+            /"([^"]+)"/g,
+            `"<span class="quoted-text" line_number=${lineNumber} onclick="copyElementToClipboard(this)">$1</span>"`
+        );
+        line += ` <a  id="a-${lineCounter}" href="javascript:openInVsCode(document.getElementById(\`a-${lineCounter}\`))"
+                        title="open in VS Code"
+                        file_name="${filename}"
+                        line_number="${lineNumber}"> &uarr; </a>`;
+    } else if (matchesStringRegex) {
+        line = line.replace(/"([^"]+)"/g, '"<span class="quoted-text" onclick="copyElementToClipboard(this)">$1</span>"');
+    } else if (containsUrlRegex.test(line)) {
+        const urlRegex = /\bhttps?:\/\/[^/]+(\/[^/]+)*\b(?=\))/g;
+        const url = line.match(urlRegex) ? line.match(urlRegex)[0] : null;
+        line = line.replace(urlRegex, `<span class="url" onclick="copyElementToClipboard(this)">$&</span>`);
+        if (url) {
+            line += ` <a  id="a-${lineCounter}" href="javascript:openInVsCode(document.getElementById(\`a-${lineCounter}\`))"
+                        title="open in VS Code"
+                        file_name="${url}"> &uarr; </a>`;
+        }
+    }
+
+    line = line.replace(/'([^']+)'/g, `'<span class="quoted-text" onclick="copyElementToClipboard(this)">$1</span>'`);
+    return line;
+}
+
+/**
+ * Colors the log lines based on the log level that
+ * are extracted from the [LVL:XX] prefix.
+ * @param {string} line
+ * @returns
+ */
+function colorLogLevels(line) {
+    const prefixPattern = /\[LVL:(\d+)\]/;
+    const prefixMatch = line.match(prefixPattern);
+    if (prefixMatch) {
+        const fullMatch = prefixMatch[0];
+        const logLevel = parseInt(prefixMatch[1]);
+        if (logLevel >= 50) {
+            line = line.replace(fullMatch, `</span><span id="error-${state.errorCounter}" class="critical">`);
+            state.errorCounter++;
+        } else if (logLevel >= 40) {
+            line = line.replace(fullMatch, `</span><span id="error-${state.errorCounter}" class="error">`);
+            state.errorCounter++;
+        } else if (logLevel >= 30) {
+            line = line.replace(fullMatch, `</span><span class="warning">`);
+            state.warningCounter++;
+        } else if (logLevel >= 20) {
+            line = line.replace(fullMatch, `</span><span class="info">`);
+        } else {
+            line = line.replace(fullMatch, `</span><span class="debug">`);
+        }
+    }
+    return line;
+}
+
+/**
+ * Renders the log text - highlights errors, warnings, and info messages.
+ * Adds line numbers to the log text.
+ * @param {string[]} logLines - the log text to be rendered
+ * @returns {string} - the formatted log text as HTML
+ */
+function renderLogText(logLines) {
+    let formattedLog = "";
+    let lineCounter = 1;
+
+    state.currentError = -1;
+    state.errorCounter = 0;
+    state.warningCounter = 0;
+
+    for (let i = 0; i < logLines.length; i++) {
+        logLines[i] = renderLine(logLines[i], lineCounter) + "<br />";
+        logLines[i] = colorLogLevels(logLines[i]);
+        lineCounter++;
+    }
+    formattedLog = logLines.join("");
+    return `<span>${formattedLog}</span>`;
+}
+
+/**
+ * Returns the offset of the toolbar.
+ * @returns {number}
+ */
+function getOffset() {
+    return divToolbar.offsetHeight - 1;
+}
+
+/**
+ * Opens the file in VS Code.
+ * The invoking element must have the attributes file_name and line_number.
+ * @param {HTMLElement} element - the invoking element
+ * @returns {void}
+ */
+function openInVsCode(element) {
+    let fileName = element.getAttribute("file_name");
+    const lineNumber = element.getAttribute("line_number");
+    fileName = splitPath(fileName);
+    fileName = preservedState.stringSearchValue ?
+        fileName.replace(preservedState.stringSearchValue, preservedState.stringReplaceValue) :
+        fileName;
+    const url = lineNumber ? `vscode://file/${fileName}:${lineNumber}` : `vscode://file/${fileName}`;
+    window.open(url);
+}
+
+/**
+ * Splits the path at the splitter and returns the last part.
+ * @param {string} path
+ * @returns {string} - the last part of the path
+ */
+function splitPath(path) {
+    const prefix = inputPathPrefix.value;
+    const splitter = inputPathSplitter.value;
+    const splitted = path.split(splitter);
+    if (!splitter) {
+        return path;
+    } else if (splitted.length > 1) {
+        return prefix + splitted[splitted.length - 1];
+    }
+    return splitted[splitted.length - 1];
+}
+
+/**
+ * Copies the text of the invoking element to the clipboard.
+ * If the element has a line_number attribute, it is appended to the text.
+ * @param {HTMLElement} HTMLElement - the invoking element
+ * @returns {void}
+ */
+function copyElementToClipboard(HTMLElement) {
+    const text = HTMLElement.innerText;
+    const tempInput = document.createElement("input");
+    tempInput.value = text;
+    if (inputPathSplitter) {
+        tempInput.value = splitPath(text);
+    }
+    document.body.appendChild(tempInput);
+    if (HTMLElement.hasAttribute("line_number")) {
+        tempInput.value += ":" + HTMLElement.getAttribute("line_number");
+    }
+    tempInput.select();
+    document.execCommand("copy");
+    showMessageToast(`${tempInput.value}<br/><span class="info">Copied to clipboard</span>`);
+    document.body.removeChild(tempInput);
+}
+
+/**
+ * Scrolls to the line with the given id.
+ * @param {string} id
+ * @returns {void}
+ */
+function goToLineWidId(id) {
+    const scrollOffset = getOffset();
+    try {
+        const _id = parseInt(id);
+        const line = document.getElementById("line-" + _id);
+        line.scrollIntoView();
+        window.scroll(0, window.scrollY - scrollOffset);
+    } catch {}
+}
+
+/**
+ * Scrolls start of the error with the given error number.
+ * @param {number} errorNo
+ * @returns {void}
+ */
+function goToError(errorNo) {
+    const scrollOffset = getOffset();
+    const errorElement = document.getElementById(`error-${errorNo}`);
+    const errYPos = errorElement.getBoundingClientRect().top;
+
+    if (errYPos + window.scrollY - document.body.scrollHeight > 0) {
+        window.scroll(0, document.body.scrollHeight);
+    } else {
+        errorElement.scrollIntoView();
+        window.scroll(0, window.scrollY - scrollOffset);
+    }
+
+    errorElement.style.backgroundColor = "var(--highlight-color)";
+    setTimeout(() => {
+        errorElement.style.backgroundColor = "";
+    }, state.timeout);
+}
+
+/**
+ * Scrolls to the latest error.
+ * @returns {void}
+ */
+function goToLastError() {
+    if (state.errorCounter > 0) {
+        state.currentError = state.errorCounter - 1;
+        goToError(state.currentError);
+    }
+}
+
+/**
+ * Scrolls to the next error in the log file.
+ * @returns {void}
+ */
+function goToNextError() {
+    if (state.currentError < state.errorCounter - 1) {
+        state.currentError++;
+        goToError(state.currentError);
+    }
+}
+
+/**
+ * Scrolls to the previous error in the log file.
+ * @returns {void}
+ */
+function goToPreviousError() {
+    if (state.currentError > 0) {
+        state.currentError--;
+        goToError(state.currentError);
+    }
+}
+
+/**
+ * Sets up the page:
+ * - Parses the hash so that the page can be restored to its previous state
+ * - Sets up event listeners
+ * - Fetches file paths from the server
+ * - Requests the timestamp of the log file so that the user can be notified if the log file has changed
+ */
+function setUpPage() {
+    try {
+        const hash = decodeURIComponent(window.location.hash.substring(1));
+        Object.assign(preservedState, JSON.parse(atob(hash)).preservedState);
+    } catch (error) {
+        console.debug("Did not parse hash:", error);
+    }
+
+    bindElementValue(inputPathPrefix, preservedState, "pathPrefix", true, bindingObserverFn);
+    bindElementValue(inputPathSplitter, preservedState, "pathSplitter", true, bindingObserverFn);
+    bindElementAttr(btnAutoRefresh, "state", preservedState, "autoRefreshState", true, bindingObserverFn);
+    window.onload = () => {
+        setUpEventListeners();
+        fetchFilePaths();
+        setInterval(() => {
+            requestLogfileTimestamp();
+        }, 2 * state.timeout);
+    };
+    adjustLogContentMargin();
+}
+
 setUpPage();
```

### Comparing `django-log-lens-0.1.8/django_log_lens/views.py` & `django-log-lens-0.1.9/django_log_lens/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,152 @@
-import json
-import logging
-import os
-
-from django.conf import settings
-from django.contrib.auth import authenticate, login, logout
-from django.contrib.auth.decorators import user_passes_test
-from django.http import HttpResponse, HttpResponseBadRequest, JsonResponse
-from django.shortcuts import redirect, render
-from django.views.decorators.http import require_http_methods
-
-HANDLER_NAME_NOT_PROVIDED_TEXT = "400 Bad Request: no handler name provided"
-
-try:
-    ALLOW_JS_LOGGING = settings.ALLOW_JS_LOGGING
-except AttributeError:
-    ALLOW_JS_LOGGING = False
-
-client_logger = logging.getLogger("django_log_lens.client")
-
-log_level_functional_map = {
-    "DEBUG": client_logger.debug,
-    "INFO": client_logger.info,
-    "WARNING": client_logger.warning,
-    "ERROR": client_logger.error,
-    "CRITICAL": client_logger.critical,
-    "ASSERTION FAILED (CRITICAL)": client_logger.critical
-}
-
-
-@require_http_methods(["POST"])
-def logout_view(request):
-    if request.user.is_authenticated:
-        logout(request)
-    return redirect('log-lens:login')
-
-
-@require_http_methods(["GET", "POST"])
-def login_view(request):
-    if request.method == 'POST':
-        username = request.POST.get('username', '')
-        password = request.POST.get('password', '')
-        user = authenticate(username=username, password=password)
-        if user is not None and user.is_superuser:  # type: ignore
-            login(request, user)
-            return redirect('log-lens:view')
-        elif user is not None:
-            return render(request, 'log-lens-login.html', {'error_message': f'{username} is not a superuser'})
-        else:
-            return render(request, 'log-lens-login.html', {'error_message': 'Invalid credentials'})
-    else:
-        return render(request, 'log-lens-login.html')
-
-
-@require_http_methods(["POST"])
-def log_js_error(request):
-    """Logs the error message and stack trace provided by the POST request."""
-    if not ALLOW_JS_LOGGING:
-        return HttpResponseBadRequest("JavaScript / Client logging is not allowed")
-
-    log = json.loads(request.body.decode('utf-8'))
-    log_message = log['error_message']
-    log_level = log['severity']
-    log_level_functional_map.get(log_level, client_logger.error)(log_message)
-    return HttpResponse("Log message processed.")
-
-
-@require_http_methods(["GET"])
-@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
-def request_logfile(request) -> HttpResponse:
-    """
-    Returns the contents of the log file specified by the handler_name GET parameter.
-    A logged in superuser is required.
-    """
-    handler_name = request.GET.get('handler_name', None)
-    if handler_name is None:
-        return HttpResponseBadRequest(HANDLER_NAME_NOT_PROVIDED_TEXT)
-    try:
-        filename = settings.LOGGING['handlers'][handler_name]['filename']
-        with open(filename, 'r') as f:
-            ti_m = os.path.getmtime(filename)
-            return JsonResponse({"text": f.read(), "timestamp": f"{ti_m}"})
-    except (FileNotFoundError, KeyError):
-        return HttpResponse("No logs available")
-
-
-@require_http_methods(["GET"])
-@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
-def request_logfile_timestamp(request) -> HttpResponse:
-    """
-    Returns the contents of the log file specified by the handler_name GET parameter.
-    A logged in superuser is required.
-    """
-    handler_name = request.GET.get('handler_name', None)
-    if handler_name is None:
-        return HttpResponseBadRequest(HANDLER_NAME_NOT_PROVIDED_TEXT)
-    try:
-        filename = settings.LOGGING['handlers'][handler_name]['filename']
-        ti_m = os.path.getmtime(filename)
-        return JsonResponse({"timestamp": f"{ti_m}"})
-    except (FileNotFoundError, KeyError):
-        return JsonResponse({})
-
-
-@require_http_methods(["DELETE"])
-@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
-def clear_logfile(request) -> HttpResponse:
-    """
-    Clears the contents of the log file specified by the handler_name GET parameter.
-    A logged in superuser is required.
-    """
-    handler_name = request.GET.get('handler_name', None)
-    if handler_name is None:
-        return HttpResponseBadRequest(HANDLER_NAME_NOT_PROVIDED_TEXT)
-    filename = settings.LOGGING['handlers'][handler_name]['filename']
-    try:
-        with open(filename, 'w') as f:
-            f.write("")
-            return HttpResponse(f"Log file {filename} cleared")
-    except FileNotFoundError:
-        return HttpResponse("No logs available")
-
-
-@require_http_methods(["GET"])
-@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
-def request_logfile_paths(request) -> JsonResponse | HttpResponseBadRequest:
-    """
-    Returns a JSON object containing the paths of all log files.
-    A logged in superuser is required.
-    """
-    try:
-        paths = {}
-        for handler_name in settings.LOGGING['handlers']:
-            if 'filename' in settings.LOGGING['handlers'][handler_name]:
-                paths[handler_name] = settings.LOGGING['handlers'][handler_name]['filename']
-        return JsonResponse(paths)
-    except KeyError:
-        return JsonResponse({})
-
-
-@require_http_methods(["GET"])
-@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
-def log_lens_view(request) -> HttpResponse:
-    """
-    Returns the log viewer page.
-    A logged in superuser is required.
-    """
-    return render(request, 'log-lens.html')
+import json
+import logging
+import os
+
+from django.conf import settings
+from django.contrib.auth import authenticate, login, logout
+from django.contrib.auth.decorators import user_passes_test
+from django.http import HttpResponse, HttpResponseBadRequest, JsonResponse
+from django.shortcuts import redirect, render
+from django.views.decorators.http import require_http_methods
+
+HANDLER_NAME_NOT_PROVIDED_TEXT = "400 Bad Request: no handler name provided"
+
+try:
+    ALLOW_JS_LOGGING = settings.ALLOW_JS_LOGGING
+except AttributeError:
+    ALLOW_JS_LOGGING = False
+
+client_logger = logging.getLogger("django_log_lens.client")
+
+log_level_functional_map = {
+    "DEBUG": client_logger.debug,
+    "INFO": client_logger.info,
+    "WARNING": client_logger.warning,
+    "ERROR": client_logger.error,
+    "CRITICAL": client_logger.critical,
+    "ASSERTION FAILED (CRITICAL)": client_logger.critical
+}
+
+
+@require_http_methods(["POST"])
+def logout_view(request):
+    if request.user.is_authenticated:
+        logout(request)
+    return redirect('log-lens:login')
+
+
+@require_http_methods(["GET", "POST"])
+def login_view(request):
+    if request.method == 'POST':
+        username = request.POST.get('username', '')
+        password = request.POST.get('password', '')
+        user = authenticate(username=username, password=password)
+        if user is not None and user.is_superuser:  # type: ignore
+            login(request, user)
+            return redirect('log-lens:view')
+        elif user is not None:
+            return render(request, 'log-lens-login.html', {'error_message': f'{username} is not a superuser'})
+        else:
+            return render(request, 'log-lens-login.html', {'error_message': 'Invalid credentials'})
+    else:
+        return render(request, 'log-lens-login.html')
+
+
+@require_http_methods(["POST"])
+def log_js_error(request):
+    """Logs the error message and stack trace provided by the POST request."""
+    if not ALLOW_JS_LOGGING:
+        return HttpResponseBadRequest("JavaScript / Client logging is not allowed")
+
+    log = json.loads(request.body.decode('utf-8'))
+    log_message = log['error_message']
+    log_level = log['severity']
+    log_level_functional_map.get(log_level, client_logger.error)(log_message)
+    return HttpResponse("Log message processed.")
+
+
+@require_http_methods(["GET"])
+@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
+def request_logfile(request) -> HttpResponse:
+    """
+    Returns the contents of the log file specified by the handler_name GET parameter.
+    A logged in superuser is required.
+    """
+    handler_name = request.GET.get('handler_name', None)
+    if handler_name is None:
+        return HttpResponseBadRequest(HANDLER_NAME_NOT_PROVIDED_TEXT)
+    try:
+        filename = settings.LOGGING['handlers'][handler_name]['filename']
+        with open(filename, 'r') as f:
+            ti_m = os.path.getmtime(filename)
+            return JsonResponse({"text": f.read(), "timestamp": f"{ti_m}"})
+    except FileNotFoundError:
+        return JsonResponse({"text": f"Log file {filename} not found", "timestamp": "0"})
+    except KeyError:
+        return JsonResponse(
+            {"text": "Improperly configured.\nPlease check the LOGGING configuration"
+             " in your settings.py", "timestamp": "0"})
+
+
+@require_http_methods(["GET"])
+@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
+def request_logfile_timestamp(request) -> HttpResponse:
+    """
+    Returns the contents of the log file specified by the handler_name GET parameter.
+    A logged in superuser is required.
+    """
+    handler_name = request.GET.get('handler_name', None)
+    if handler_name is None:
+        return HttpResponseBadRequest(HANDLER_NAME_NOT_PROVIDED_TEXT)
+    try:
+        filename = settings.LOGGING['handlers'][handler_name]['filename']
+        ti_m = os.path.getmtime(filename)
+        return JsonResponse({"timestamp": f"{ti_m}"})
+    except (FileNotFoundError, KeyError):
+        return JsonResponse({"timestamp": "0"})
+
+
+@require_http_methods(["DELETE"])
+@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
+def clear_logfile(request) -> HttpResponse:
+    """
+    Clears the contents of the log file specified by the handler_name GET parameter.
+    A logged in superuser is required.
+    """
+    handler_name = request.GET.get('handler_name', None)
+    if handler_name is None:
+        return HttpResponseBadRequest(HANDLER_NAME_NOT_PROVIDED_TEXT)
+    filename = settings.LOGGING['handlers'][handler_name]['filename']
+    try:
+        with open(filename, 'w') as f:
+            f.write("")
+        return HttpResponse(f"Log file {filename} cleared")
+    except FileNotFoundError:
+        return HttpResponse("No logs available")
+
+
+@require_http_methods(["GET"])
+@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
+def request_logfile_paths(request) -> JsonResponse | HttpResponseBadRequest:
+    """
+    Returns a JSON object containing the paths of all log files.
+    A logged in superuser is required.
+    """
+    try:
+        paths = {}
+        for handler_name in settings.LOGGING['handlers']:
+            if 'filename' in settings.LOGGING['handlers'][handler_name]:
+                paths[handler_name] = settings.LOGGING['handlers'][handler_name]['filename']
+        return JsonResponse(paths)
+    except KeyError:
+        return JsonResponse({})
+
+
+@require_http_methods(["GET"])
+@user_passes_test(lambda user: user.is_superuser, login_url='log-lens:login')
+def log_lens_view(request) -> HttpResponse:
+    """
+    Returns the log viewer page.
+    A logged in superuser is required.
+    """
+    return render(request, 'log-lens.html')
```

### Comparing `django-log-lens-0.1.8/django_log_lens.egg-info/PKG-INFO` & `django-log-lens-0.1.9/django_log_lens.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,118 @@
-Metadata-Version: 2.1
-Name: django-log-lens
-Version: 0.1.8
-Summary: A lightweight Django app for viewing and managing log data conveniently
-Home-page: https://github.com/martinbroede/django-log-lens
-Author: Martin Broede
-Author-email: martin.broede@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[![PyPi](https://img.shields.io/badge/PyPi-django--log--lens-blue)](https://pypi.org/project/django-log-lens/)
-[![Version](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmartinbroede%2Fdjango-log-lens%2Fmain%2FVERSION.json&query=version&label=Latest%20Version)](https://raw.githubusercontent.com/martinbroede/django-log-lens/main/VERSION.json)
-[![linting](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml/badge.svg)](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml)
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-
-<br>
-
-<img width="830px" src="https://raw.githubusercontent.com/martinbroede/django-log-lens/main/django_log_lens/static/django_log_lens/logo.svg">
-
-<br>
-
-Django Log Lens is a Django app that provides a simple, lightweight and easy-to-use logging system for your Django project.
-
-
-## Getting Started
-
-### 1. Install `django-log-lens` from PyPi
-
-```
-pip install django-log-lens
-```
-
-### 2. Add `django_log_lens` to your `INSTALLED_APPS`
-
-```python
-# file: settings.py
-
-INSTALLED_APPS = [
-    'django_log_lens',
-    ...
-]
-```
-
-### 3. Add URL patterns to your `urls.py`
-
-```python
-# file: urls.py
-from django.urls import include
-
-urlpatterns = [
-    path('logs/', include('django_log_lens.urls')),
-    ...
-]
-```
-
-### 4. Add a `LOGGING` configuration in your `settings.py`
-
-Follow the instructions from the [official Django documentation](https://docs.djangoproject.com/en/5.0/topics/logging/#configuring-logging) to configure the logging system or use the example below.
-
-```python
-# file: settings.py
-from django_log_lens import LOG_FORMAT
-
-LOG_FOLDER = BASE_DIR / "logs"
-
-if not os.path.exists(LOG_FOLDER):
-    os.makedirs(LOG_FOLDER)
-
-LOGGING = {
-    "version": 1,
-    "disable_existing_loggers": False,
-    "formatters": {"default": {"format": LOG_FORMAT}},
-    "handlers": {
-        "log_collector": {
-            "level": "WARNING",
-            "class": "logging.FileHandler",
-            "filename": str(LOG_FOLDER / "collector.log"),
-            "formatter": "default",
-        },
-        "client_logger": {
-            "level": "DEBUG",
-            "class": "logging.FileHandler",
-            "filename": str(LOG_FOLDER / "client.log"),
-            "formatter": "default",
-        },
-    },
-    "loggers": {
-        "django_log_lens.client": {"handlers": ["client_logger"], "level": "DEBUG", "propagate": True},
-        "django" : {"handlers": ["log_collector"], "level": "DEBUG", "propagate": True},
-    }
-}
-
-ALLOW_JS_LOGGING = True  # django_log_lens setting: allows clients to send console logs to the server
-```
-
-### 5. Visit Log Lens
-
-You can now visit Django Log Lens by navigating to `{% url 'django_log_lens:view' %}` (code for your template) -
- if you configured the URL pattern as shown above, this would be `logs/view`
-
-
-## Third Party Licenses
-
-This project uses the Dracula theme by Zeno Rocha which is
-licensed under the [MIT License](https://raw.githubusercontent.com/dracula/dracula-theme/main/LICENSE)
+Metadata-Version: 2.1
+Name: django-log-lens
+Version: 0.1.9
+Summary: A lightweight Django app for viewing and managing log data conveniently
+Home-page: https://github.com/martinbroede/django-log-lens
+Author: Martin Broede
+Author-email: martin.broede@gmail.com
+Maintainer: Martin Broede
+Maintainer-email: martin.broede@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![PyPI](https://img.shields.io/badge/PyPI-django--log--lens-blue)](https://pypi.org/project/django-log-lens/)
+[![Version](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmartinbroede%2Fdjango-log-lens%2Fmain%2FVERSION.json&query=version&label=Latest%20Version)](https://raw.githubusercontent.com/martinbroede/django-log-lens/main/VERSION.json)
+[![linting](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml/badge.svg)](https://github.com/martinbroede/django-log-lens/actions/workflows/linting.yaml)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+<br>
+
+<img width="830px" src="https://raw.githubusercontent.com/martinbroede/django-log-lens/main/django_log_lens/static/django_log_lens/logo.svg">
+
+<br>
+
+Django Log Lens is a Django app that provides a simple, lightweight and easy-to-use logging system for your Django project.
+
+
+## Getting Started
+
+### 1. Install `django-log-lens` from PyPI
+
+```
+pip install django-log-lens
+```
+
+### 2. Add `django_log_lens` to your `INSTALLED_APPS`
+
+```python
+# file: settings.py
+
+INSTALLED_APPS = [
+    'django_log_lens',
+    ...
+]
+```
+
+### 3. Add URL patterns to your `urls.py`
+
+```python
+# file: urls.py
+from django.urls import include
+
+urlpatterns = [
+    path('logs/', include('django_log_lens.urls')),
+    ...
+]
+```
+
+### 4. Add a `LOGGING` configuration in your `settings.py`
+
+Follow the instructions from the [official Django documentation](https://docs.djangoproject.com/en/5.0/topics/logging/#configuring-logging) to configure the logging system or use the example below.
+
+```python
+# file: settings.py
+from django_log_lens import LOG_FORMAT
+
+LOG_FOLDER = BASE_DIR / "logs"
+
+if not os.path.exists(LOG_FOLDER):
+    os.makedirs(LOG_FOLDER)
+
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "formatters": {"default": {"format": LOG_FORMAT}},
+    "handlers": {
+        "log_collector": {
+            "level": "WARNING",
+            "class": "logging.FileHandler",
+            "filename": str(LOG_FOLDER / "collector.log"),
+            "formatter": "default",
+        },
+        "client_logger": {
+            "level": "DEBUG",
+            "class": "logging.FileHandler",
+            "filename": str(LOG_FOLDER / "client.log"),
+            "formatter": "default",
+        },
+    },
+    "loggers": {
+        "django_log_lens.client": {"handlers": ["client_logger"], "level": "DEBUG", "propagate": True},
+        "django" : {"handlers": ["log_collector"], "level": "DEBUG", "propagate": True},
+    }
+}
+
+ALLOW_JS_LOGGING = True  # django_log_lens setting: allows clients to send console logs to the server
+```
+
+### 5. Visit Log Lens
+
+You can now visit Django Log Lens by navigating to `{% url 'django_log_lens:view' %}` (code for your template) -
+ if you configured the URL pattern as shown above, this would be `logs/view`
+
+
+## Third Party Licenses
+
+This project uses the Dracula theme by Zeno Rocha which is
+licensed under the [MIT License](https://raw.githubusercontent.com/dracula/dracula-theme/main/LICENSE)
+
```

### Comparing `django-log-lens-0.1.8/django_log_lens.egg-info/SOURCES.txt` & `django-log-lens-0.1.9/django_log_lens.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 django_log_lens/__init__.py
 django_log_lens/apps.py
 django_log_lens/urls.py
 django_log_lens/views.py
 django_log_lens.egg-info/PKG-INFO
 django_log_lens.egg-info/SOURCES.txt
 django_log_lens.egg-info/dependency_links.txt
+django_log_lens.egg-info/requires.txt
 django_log_lens.egg-info/top_level.txt
-django_log_lens/static/django_log_lens/favicon-cyan.svg
 django_log_lens/static/django_log_lens/favicon.svg
 django_log_lens/static/django_log_lens/logger.js
 django_log_lens/static/django_log_lens/logo.svg
 django_log_lens/static/django_log_lens/script.js
 django_log_lens/static/django_log_lens/styles.css
 django_log_lens/templates/js-logger.html
 django_log_lens/templates/log-lens-login.html
```

