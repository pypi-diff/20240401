# Comparing `tmp/djsm-0.1.5.tar.gz` & `tmp/djsm-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsm-0.1.5.tar", last modified: Mon Jan 29 20:04:35 2024, max compression
+gzip compressed data, was "djsm-0.1.51.tar", last modified: Mon Apr  1 19:32:59 2024, max compression
```

## Comparing `djsm-0.1.5.tar` & `djsm-0.1.51.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 20:04:35.599220 djsm-0.1.5/
--rw-rw-rw-   0        0        0     1104 2024-01-13 20:04:07.000000 djsm-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     8082 2024-01-29 20:04:35.599220 djsm-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6900 2024-01-13 19:50:41.000000 djsm-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-01-29 20:04:35.458606 djsm-0.1.5/djsm/
--rw-rw-rw-   0        0        0      871 2024-01-29 20:02:22.000000 djsm-0.1.5/djsm/__init__.py
--rw-rw-rw-   0        0        0      146 2024-01-10 18:54:51.000000 djsm-0.1.5/djsm/apps.py
--rw-rw-rw-   0        0        0      205 2024-01-02 16:50:52.000000 djsm-0.1.5/djsm/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-01-29 20:04:35.380453 djsm-0.1.5/djsm/management/
-drwxrwxrwx   0        0        0        0 2024-01-29 20:04:35.599220 djsm-0.1.5/djsm/management/commands/
--rw-rw-rw-   0        0        0      642 2024-01-13 19:04:30.000000 djsm-0.1.5/djsm/management/commands/change_cryptkeys.py
--rw-rw-rw-   0        0        0      658 2024-01-13 19:04:10.000000 djsm-0.1.5/djsm/management/commands/djsm_cleanup.py
--rw-rw-rw-   0        0        0      635 2024-01-13 19:17:24.000000 djsm-0.1.5/djsm/management/commands/djsm_reload_env.py
--rw-rw-rw-   0        0        0     1329 2024-01-29 19:57:43.000000 djsm-0.1.5/djsm/management/commands/update_secrets.py
--rw-rw-rw-   0        0        0     7107 2024-01-13 20:34:47.000000 djsm-0.1.5/djsm/management/commands/use_djsm.py
--rw-rw-rw-   0        0        0    12724 2024-01-13 18:54:48.000000 djsm-0.1.5/djsm/manager.py
--rw-rw-rw-   0        0        0     2686 2024-01-13 12:27:28.000000 djsm-0.1.5/djsm/misc.py
-drwxrwxrwx   0        0        0        0 2024-01-29 20:04:35.599220 djsm-0.1.5/djsm.egg-info/
--rw-rw-rw-   0        0        0     8082 2024-01-29 20:04:35.000000 djsm-0.1.5/djsm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-01-29 20:04:35.000000 djsm-0.1.5/djsm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 20:04:35.000000 djsm-0.1.5/djsm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-01-29 20:04:35.000000 djsm-0.1.5/djsm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-01-29 20:04:35.000000 djsm-0.1.5/djsm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1327 2024-01-13 20:04:52.000000 djsm-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-29 20:04:35.599220 djsm-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 19:32:59.042087 djsm-0.1.51/
+-rw-rw-rw-   0        0        0     1104 2024-01-13 20:04:07.000000 djsm-0.1.51/LICENSE
+-rw-rw-rw-   0        0        0     7464 2024-04-01 19:32:59.042087 djsm-0.1.51/PKG-INFO
+-rw-rw-rw-   0        0        0     6286 2024-04-01 18:58:08.000000 djsm-0.1.51/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 19:32:58.961509 djsm-0.1.51/djsm/
+-rw-rw-rw-   0        0        0      872 2024-04-01 19:32:26.000000 djsm-0.1.51/djsm/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-01-10 18:54:51.000000 djsm-0.1.51/djsm/apps.py
+-rw-rw-rw-   0        0        0      205 2024-01-02 16:50:52.000000 djsm-0.1.51/djsm/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:32:58.937231 djsm-0.1.51/djsm/management/
+drwxrwxrwx   0        0        0        0 2024-04-01 19:32:59.034085 djsm-0.1.51/djsm/management/commands/
+-rw-rw-rw-   0        0        0      641 2024-04-01 18:50:42.000000 djsm-0.1.51/djsm/management/commands/change_cryptkeys.py
+-rw-rw-rw-   0        0        0      657 2024-04-01 18:50:57.000000 djsm-0.1.51/djsm/management/commands/djsm_cleanup.py
+-rw-rw-rw-   0        0        0      634 2024-04-01 18:51:15.000000 djsm-0.1.51/djsm/management/commands/djsm_reload_env.py
+-rw-rw-rw-   0        0        0     1328 2024-04-01 18:51:22.000000 djsm-0.1.51/djsm/management/commands/update_secrets.py
+-rw-rw-rw-   0        0        0     7714 2024-04-01 19:25:21.000000 djsm-0.1.51/djsm/management/commands/use_djsm.py
+-rw-rw-rw-   0        0        0    12811 2024-04-01 19:03:50.000000 djsm-0.1.51/djsm/manager.py
+-rw-rw-rw-   0        0        0     2725 2024-04-01 19:02:10.000000 djsm-0.1.51/djsm/misc.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:32:59.034085 djsm-0.1.51/djsm.egg-info/
+-rw-rw-rw-   0        0        0     7464 2024-04-01 19:32:58.000000 djsm-0.1.51/djsm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-04-01 19:32:58.000000 djsm-0.1.51/djsm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:32:58.000000 djsm-0.1.51/djsm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-01 19:32:58.000000 djsm-0.1.51/djsm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-01 19:32:58.000000 djsm-0.1.51/djsm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1322 2024-04-01 17:59:33.000000 djsm-0.1.51/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:32:59.042087 djsm-0.1.51/setup.cfg
```

### Comparing `djsm-0.1.5/LICENSE` & `djsm-0.1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `djsm-0.1.5/PKG-INFO` & `djsm-0.1.51/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.1.5
-Summary: Light weight module that allows you to store secrets encrypted in JSON and access them easily in your Django project.
+Version: 0.1.51
+Summary: Django package that allows you to store secrets encrypted in JSON and access them easily in your Django project.
 Author-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Maintainer-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
 Classifier: Programming Language :: Python :: 3
@@ -21,67 +21,38 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv>=0.19.2
 Requires-Dist: simple-file-handler>=0.0.1
 Requires-Dist: dcrypt>=0.0.1
 
-## DJSM - Django JSON Secrets Manager
+# DJSM - Django JSON Secrets Manager
 
-Light weight Python module that allows you to easily store and access your Django project's secrets like secret key, database password, etc., encrypted in a JSON file.
+Django package that allows you to easily store and access your Django project's secrets like secret key, database password, etc., encrypted in a JSON file.
 
 [View package on PyPI](https://pypi.org/project/djsm/)
 
 ## Installation and Quick Setup
 
 * Install the package using pip.
 
 ```bash
 pip install djsm
 ```
 
 * Setup or update a '.env' file for your project.
 
-Copy this into a .env file just outside your project (adjust as needed)
-
 ```.env
-DJSM_SECRETS_FILE_PATH = "./.secretfolder/path/secrets.json" 
+DJSM_SECRETS_FILE_PATH = "./.enc/path/secrets.json" 
 # Assign path to file you want secrets to be stored in. Even if it does not exist yet
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "secretkey"
 ```
 
-Your project structure should look like this:
-
-```bash
-|-- my_project
-|   |-- my_project
-|   |   |-- __init__.py
-|   |   |-- settings.py
-|   |   |-- urls.py
-|   |   |-- wsgi.py
-|   |
-|   |-- my_app
-|   |   |-- __init__.py
-|   |   |-- admin.py
-|   |   |-- apps.py
-|   |   |-- models.py
-|   |   |-- tests.py
-|   |   |-- views.py
-|   |
-|   |-- db.sqlite3
-|   |-- manage.py
-|   |-- .gitignore
-|   |-- requirements.txt
-|
-|-- venv
-|-- .env
-```
-
 * Import the package in your Django project
 
 In settings.py:
 
 ```python
 import djsm
 
@@ -94,22 +65,21 @@
 python manage.py runserver
 ```
 
 If everything was setup successfully, you should see "Setup OK!" on the terminal. Remember to remove the `djsm.check_setup()` line from your settings.py file.
 
 ## Usage
 
-Before starting, a '.env' file has to be created just outside the django project directory.
-In the file, the following should be added;
+Before starting, a '.env' file has to be created. In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
-SECRETS_FILE_PATH = "/.secrets/pathtofile/secrets.json"
+DJSM_SECRETS_FILE_PATH = "/.enc/pathtofile/secrets.json"
 ```
 
 * **`DJSM_SECRET_KEY_NAME`** -> Name with which the Django secret key should be stored.
 Example:
 
 ```.env
 DJSM_SECRET_KEY_NAME = 'django_secret_key'
@@ -262,15 +232,15 @@
 
 * `clean_up_and_reload()` -> Calls the `clean_up()` and `reload_env()` methods.
 
 ```python
 from djsm import DJSM  # DJSM is an alias for DjangoJSONSecretManager
 
 # Create a DJSM object
-secrets_manager = DJSM('./.secretfolder/secrets.json')
+secrets_manager = DJSM('./.enc/secrets.json')
 ```
 
 **DO NOT DELETE `cryptkeys.json` or any of the encryption keys. IF YOU DO, ALL ENCRYPTED SECRET WILL BE LOST**
 
 > NOTE: DJSM just provides an added layer of security in managing secrets in your application. It is not proven to be completely attack proof.
 
 Contributions are welcome. Please fork the repository and submit a pull request.
```

### Comparing `djsm-0.1.5/README.md` & `djsm-0.1.51/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,31 @@
-## DJSM - Django JSON Secrets Manager
+# DJSM - Django JSON Secrets Manager
 
-Light weight Python module that allows you to easily store and access your Django project's secrets like secret key, database password, etc., encrypted in a JSON file.
+Django package that allows you to easily store and access your Django project's secrets like secret key, database password, etc., encrypted in a JSON file.
 
 [View package on PyPI](https://pypi.org/project/djsm/)
 
 ## Installation and Quick Setup
 
 * Install the package using pip.
 
 ```bash
 pip install djsm
 ```
 
 * Setup or update a '.env' file for your project.
 
-Copy this into a .env file just outside your project (adjust as needed)
-
 ```.env
-DJSM_SECRETS_FILE_PATH = "./.secretfolder/path/secrets.json" 
+DJSM_SECRETS_FILE_PATH = "./.enc/path/secrets.json" 
 # Assign path to file you want secrets to be stored in. Even if it does not exist yet
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "secretkey"
 ```
 
-Your project structure should look like this:
-
-```bash
-|-- my_project
-|   |-- my_project
-|   |   |-- __init__.py
-|   |   |-- settings.py
-|   |   |-- urls.py
-|   |   |-- wsgi.py
-|   |
-|   |-- my_app
-|   |   |-- __init__.py
-|   |   |-- admin.py
-|   |   |-- apps.py
-|   |   |-- models.py
-|   |   |-- tests.py
-|   |   |-- views.py
-|   |
-|   |-- db.sqlite3
-|   |-- manage.py
-|   |-- .gitignore
-|   |-- requirements.txt
-|
-|-- venv
-|-- .env
-```
-
 * Import the package in your Django project
 
 In settings.py:
 
 ```python
 import djsm
 
@@ -67,22 +38,21 @@
 python manage.py runserver
 ```
 
 If everything was setup successfully, you should see "Setup OK!" on the terminal. Remember to remove the `djsm.check_setup()` line from your settings.py file.
 
 ## Usage
 
-Before starting, a '.env' file has to be created just outside the django project directory.
-In the file, the following should be added;
+Before starting, a '.env' file has to be created. In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
-SECRETS_FILE_PATH = "/.secrets/pathtofile/secrets.json"
+DJSM_SECRETS_FILE_PATH = "/.enc/pathtofile/secrets.json"
 ```
 
 * **`DJSM_SECRET_KEY_NAME`** -> Name with which the Django secret key should be stored.
 Example:
 
 ```.env
 DJSM_SECRET_KEY_NAME = 'django_secret_key'
@@ -235,15 +205,15 @@
 
 * `clean_up_and_reload()` -> Calls the `clean_up()` and `reload_env()` methods.
 
 ```python
 from djsm import DJSM  # DJSM is an alias for DjangoJSONSecretManager
 
 # Create a DJSM object
-secrets_manager = DJSM('./.secretfolder/secrets.json')
+secrets_manager = DJSM('./.enc/secrets.json')
 ```
 
 **DO NOT DELETE `cryptkeys.json` or any of the encryption keys. IF YOU DO, ALL ENCRYPTED SECRET WILL BE LOST**
 
 > NOTE: DJSM just provides an added layer of security in managing secrets in your application. It is not proven to be completely attack proof.
 
 Contributions are welcome. Please fork the repository and submit a pull request.
```

### Comparing `djsm-0.1.5/djsm/__init__.py` & `djsm-0.1.51/djsm/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #### djsm - Django JSON Secrets Manager
 
 Create, store, retrieve, update and manage secrets in your Django project.
 
 @Author: Daniel T. Afolayan (ti-oluwa.github.io)
 """
 
-__version__ = "0.1.5"
+__version__ = "0.1.51"
 __author__ = "Daniel T. Afolayan (ti-oluwa)"
 __license__ = "MIT"
 
 import os
 import sys
 
 from .manager import DJSM
```

### Comparing `djsm-0.1.5/djsm/management/commands/change_cryptkeys.py` & `djsm-0.1.51/djsm/management/commands/change_cryptkeys.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     Changes the encryption and decryption keys used by secrets manager.
     '''
 
     def handle(self, *args, **options) -> None:
         manager = djsm.get_djsm(quiet=True)
         manager.change_cryptkeys()
         self.stdout.write(
-            self.style.SUCCESS(f'DJSM: Encryption keys change was successfully!')
+            self.style.SUCCESS('DJSM: Encryption keys change was successfully!')
         )
         return None
```

### Comparing `djsm-0.1.5/djsm/management/commands/djsm_cleanup.py` & `djsm-0.1.51/djsm/management/commands/djsm_cleanup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     Delete the secrets (project secret key inclusive) and removes environment variables set by secrets manager.
     '''
 
     def handle(self, *args, **options) -> None:
         manager = djsm.get_djsm(quiet=True)
         manager.clean_up()
         self.stdout.write(
-            self.style.SUCCESS(f'DJSM: Clean up completed!')
+            self.style.SUCCESS('DJSM: Clean up completed!')
         )
         return None
```

### Comparing `djsm-0.1.5/djsm/management/commands/djsm_reload_env.py` & `djsm-0.1.51/djsm/management/commands/djsm_reload_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     Reloads configurations defined in the .env file into the environment variables.
     '''
 
     def handle(self, *args, **options) -> None:
         manager = djsm.get_djsm(quiet=True)
         manager.reload_env()
         self.stdout.write(
-            self.style.SUCCESS(f'DJSM: Reload complete!')
+            self.style.SUCCESS('DJSM: Reload complete!')
         )
         return None
```

### Comparing `djsm-0.1.5/djsm/management/commands/update_secrets.py` & `djsm-0.1.51/djsm/management/commands/update_secrets.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     def handle(self, *args, **options) -> None:
         name = options['name']
         value = options['value']
 
         manager = djsm.get_djsm(quiet=True)
         manager.update_secrets({name: value})
         self.stdout.write(
-            self.style.SUCCESS(f'DJSM: Secrets updated successfully!')
+            self.style.SUCCESS('DJSM: Secrets updated successfully!')
         )
         return None
```

### Comparing `djsm-0.1.5/djsm/management/commands/use_djsm.py` & `djsm-0.1.51/djsm/management/commands/use_djsm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.core.management.base import BaseCommand
-from django.conf import settings
+from django.conf import settings, Settings
 import simple_file_handler as sfh
 from typing import List
 import re
 from django.utils.module_loading import import_string
 
 from ...manager import DJSM
 
 
-def get_settings_filepath():
+def get_settings_filepath() -> str | None:
     """Return the path to the project's settings file."""
     try:
         settings.configure()
     except RuntimeError:
         pass
 
     settings_module = settings.SETTINGS_MODULE
@@ -29,62 +29,70 @@
     """
     possible_imports = ('djsm', 'DJSM', 'DjangoJSONSecretsManager')
     for line in settings_lines:
         # Ignore comments and blank lines and docstrings.
         if line.startswith(("#", "'''", '"""')) or line.strip() == '':
             continue
         # Ignore lines that are not imports.
-        if not line.startswith(('import', 'from')):
+        if not line.startswith(('import ', 'from ')):
             continue
         # If any of the possible imports are in the line, return True.
         if any(map(lambda x: x in line, possible_imports)):
             return True
     return False
 
 
-def get_djsm_obj_name_in_settings() -> DJSM | None:
+def get_djsm_obj_name_in_settings() -> str | None:
     """
     Return the name of the DJSM object in the project's settings file, If there is one.
 
     If there is no DJSM object in the project's settings file, return None.
     """
-    settings_module = import_string(settings.SETTINGS_MODULE)
+    settings_module: Settings = import_string(settings.SETTINGS_MODULE)
     for name, obj in settings_module.__dict__.items():
         if isinstance(obj, DJSM):
             return name
     return None
 
 
 def get_secret_key_line_index(settings_lines: List[str]) -> int:
     """
     Return the index of the line in the project's settings file that contains the secret key.
 
     :param settings_lines: list containing the lines of the project's settings file.
     :return: The index of the line in the project's settings file that contains the secret key.
     Returns -1 if there is no such line.
     """
-    pattern = re.compile(r'^SECRET_KEY\s*=\s*[\'"]+.*[\'"]+\s*$')
-    for index, line in enumerate(settings_lines):
+    pattern = re.compile(r'^SECRET_KEY\s*=\s*.*\s*$')
+    # Iterate through the lines in reverse order, 
+    # so the last definition of the `SECRET_KEY` setting is replaced
+    for i in range(len(settings_lines) - 1, -1, -1):
+        line = settings_lines[i].strip()
         if pattern.match(line):
-            return index
+            return i
     return -1
 
 
 def get_index_of_line_after_top_imports(settings_lines: List[str]) -> int:
     """
     Return the index of the line after the imports in the project's settings file.
 
     :param settings_lines: list containing the lines of the project's settings file.
     :return: The index of the line after the imports in the project's settings file.
     Returns 0 if there are no lines or imports in the project's settings file.
+
+    NOTE: This does not factor in imports that a wrapped in a try-except block
     """
     for index, line in enumerate(settings_lines):
-        if line.strip() == '':
+        line = line.strip()
+        # If the line is empty, a comment or a docstring line, skip it
+        if not line or line.startswith(("#", "'''", '"""')):
             continue
-        if line.startswith(('import', 'from')):
+        # If it is an import line, skip it
+        if line.startswith(('import ', 'from ')):
             continue
         return index
     return 0
 
 
 def manage_secret_key_with_djsm(manager_name: str, quiet: bool, command: BaseCommand) -> None:
     """
@@ -104,33 +112,36 @@
         project_name = settings.SETTINGS_MODULE.split('.')[0]
         has_been_imported = check_if_djsm_is_imported_in_settings(lines)
         djsm_obj_name = get_djsm_obj_name_in_settings()
         secret_key_line_index = get_secret_key_line_index(lines)
         index_after_top_imports = get_index_of_line_after_top_imports(lines)
         secret_key_line = f'''SECRET_KEY = {manager_name}.get_or_create_secret_key()'''
 
-        if has_been_imported and djsm_obj_name:
+        if has_been_imported is True and djsm_obj_name is not None:
             pattern = re.compile(
                 f'''^SECRET_KEY\\s*=\\s*{djsm_obj_name}\\.[a-zA-Z_]*\\(([\\'"]+[\\w]*[\\'"]+)?\\)\\s*$'''
             )
             # If the secret key line is already managed by DJSM, do nothing.
             if pattern.match(lines[secret_key_line_index]):
                 command.stdout.write(
                     command.style.SUCCESS(f'DJSM: Looks like DJSM already manages the secret key for {project_name}!')
                 )
-                return None
+                return
             lines[secret_key_line_index] = f'''SECRET_KEY = {djsm_obj_name}.get_or_create_secret_key()'''
 
-        elif has_been_imported and not djsm_obj_name:
+        elif has_been_imported is True and djsm_obj_name is None:
             setup_line = f"""{manager_name} = djsm.get_djsm(quiet={quiet})"""
             lines.insert(index_after_top_imports, setup_line)
             lines[secret_key_line_index] = secret_key_line
 
-        elif not has_been_imported and not djsm_obj_name:
-            setup_line = f"""import djsm\n\n{manager_name} = djsm.get_djsm(quiet={quiet})"""
+        elif has_been_imported is False and djsm_obj_name is None:
+            # Import package at the top of the file
+            lines.insert(0, "import djsm")
+            setup_line = f"""\n{manager_name} = djsm.get_djsm(quiet={quiet})"""
+            # Setup manager after import
             lines.insert(index_after_top_imports, setup_line)
             lines[secret_key_line_index] = secret_key_line
 
         new_content = '\n'.join(lines)
         # Overwrite the project's settings file with the new content.
         hdl.write_to_file(new_content, write_mode='w')
```

### Comparing `djsm-0.1.5/djsm/manager.py` & `djsm-0.1.51/djsm/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
     """Returns an `FileHandler` object for an .env file"""
     return sfh.FileHandler(find_dotenv(raise_error_if_not_found=True), allow_any=True) 
 
 
 
 class DjangoJSONSecretManager:
     cryptkeys_filename = 'cryptkeys.json'
+    """The default name in which the manager's cryptkeys will be stored"""
 
-    def __init__(self, path_to_secret_file: str, *, quiet: bool = False):
+    def __init__(self, path_to_secret_file: str, *, quiet: bool = False) -> None:
         """
         Creates a new DjangoJSONSecretManager object.
 
         :param path_to_secret_file: path the file where secrets are stored or secrets will be stored.
         :param quiet: If True, do not write anything to stdout (to avoid cluttering the console)
         """
         try:
@@ -46,15 +47,15 @@
                 raise ValueError('DJSM_SECRET_KEY_NAME must be a valid identifier')
             self.secret_key_name = dj_keyname
         else:
             self.secret_key_name = 'django_secret_key'
         return None
 
     @property
-    def cryptkeys_filepath(self):
+    def cryptkeys_filepath(self) -> str:
         """Returns the path to the crypt keys file"""
         return f"{os.path.dirname(self.secrets_file_path)}\\{self.cryptkeys_filename.split('.')[0]}.json"
     
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         if "path" in __name:
             if not os.path.isabs(__value):
@@ -73,19 +74,19 @@
             raise TypeError("secret must be a dict")
         
         with sfh.FileHandler(self.cryptkeys_filepath) as crypt_keys_file_hdl:
             try:
                 cryptkeys: Dict = crypt_keys_file_hdl.read_file()
                 m_key = cryptkeys.get('DJSM_MASTER_KEY', None)
                 pub_key = cryptkeys.get('DJSM_PUBLIC_KEY', None)
-            except:
+            except Exception:
                 m_key, pub_key = None, None
             priv_key = os.getenv('DJSM_PRIVATE_KEY')
 
-            if all((m_key, pub_key, priv_key)) == False:
+            if all((m_key, pub_key, priv_key)) is False:
                 key_signature = dcrypt.CryptKey.make_signature(hash_algorithm="SHA-256")
                 m_key, pub_key, priv_key, _ = key_signature.common()
                 cryptkeys = {
                     'DJSM_MASTER_KEY': m_key,
                     'DJSM_PUBLIC_KEY': pub_key,
                 }
                 crypt_keys_file_hdl.write_to_file(cryptkeys)
@@ -113,20 +114,20 @@
             raise TypeError("encrypted_secret must be a dict")
         
         with sfh.FileHandler(self.cryptkeys_filepath) as crypt_keys_file_hdl:
             try:
                 cryptkeys: Dict = crypt_keys_file_hdl.read_file()
                 m_key: str = cryptkeys.get('DJSM_MASTER_KEY', None)
                 pub_key: str = cryptkeys.get('DJSM_PUBLIC_KEY', None)
-            except:
+            except Exception:
                 m_key, pub_key = None, None
 
             priv_key: str = os.getenv('DJSM_PRIVATE_KEY')
 
-            if all((m_key, pub_key, priv_key)) == False:
+            if all((m_key, pub_key, priv_key)) is False:
                 raise CryptKeysNotFound("Crypt key(s) not found. Secrets will not be recoverable")
 
             common_signature = dcrypt.CommonSignature(m_key, pub_key, priv_key, "SHA-256")
             cryptkey = dcrypt.CryptKey(signature=dcrypt.Signature.from_common(common_signature))
             crypt = dcrypt.JSONCrypt(key=cryptkey)
             del m_key, pub_key, priv_key
             return crypt.decrypt(encrypted_secret)
@@ -189,20 +190,20 @@
             self.stdout("DJSM: Invalid Secret Key. Replacing Key...\n")
             # Replace secret key if the secret key is not valid and return the new secret key
             return self.get_or_create_secret_key(always_generate=True)
         return secret_key
 
 
     def _write_secrets(
-            self, 
-            secrets: Dict[str, Any], 
-            path_to_file: str, 
-            overwrite: bool = False, 
-            encrypt: bool = False
-        ) -> None:
+        self, 
+        secrets: Dict[str, Any], 
+        path_to_file: str, 
+        overwrite: bool = False, 
+        encrypt: bool = False
+    ) -> None:
         """
         Writes the secrets in the given path.
 
         :param secrets: dictionary containing new secrets.
         :param path_to_file: path to file in which secrets will be written into.
         :param overwrite: whether to overwrite all existing secrets in the file.
         :param encrypt: whether to encrypt the secrets before writing in the file.
```

### Comparing `djsm-0.1.5/djsm/misc.py` & `djsm-0.1.51/djsm/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
 env_variables = (
     "DJSM_SECRETS_FILE_PATH",
     "DJSM_SECRET_KEY_NAME",
 )
 
 
-def find_and_load_env_var():
+def find_and_load_env_var() -> None:
     """Load environment variables from .env file"""
     try:
         load_dotenv(find_dotenv('.env', raise_error_if_not_found=True), override=True)
     except Exception:
         raise EnvLoadError("Could not load environmental variables because '.env' file was not found. Create one!")
     return None
 
 
-def _print(msg: str, quiet: bool = False):
+def _print(msg: str, quiet: bool = False) -> None:
     if not quiet:
         sys.stdout.write(msg)
 
 
-def check_setup(quiet: bool = False):
+def check_setup(quiet: bool = False) -> bool:
     """
     Check that an .env file is present and has been properly setup
     
     :param quiet: If True, do not write anything to stdout (to avoid cluttering the console)
     :return: True if setup is OK, False if not
     """
     setup_ok = True
@@ -55,27 +55,27 @@
         load_dotenv(dotenv_path, override=True)
         _print('DJSM: Setup OK!\n', quiet=quiet)
     else:
         _print('DJSM: Visit https://github.com/ti-oluwa/djsm/#usage for help on how to setup DJSM\n')
     return setup_ok
  
 
-def validate_secret_key(secret_key: str):
+def validate_secret_key(secret_key: str) -> bool:
     """Check that Django secret key is valid."""
     if not isinstance(secret_key, str):
         return False
     if len(secret_key) < 32:
         return False
     for char in secret_key:
         if char not in SECRET_KEY_ALLOWED_CHARS:
             return False
     return True
 
 
-def generate_django_secret_key(length: int = 50):
+def generate_django_secret_key(length: int = 50) -> str:
     """
     Return a randomly generated key of not less than 32 characters
     
     :param length: length of secret key to be generated.
     """
     if length < 32:
         raise ValueError('Secret key length cannot be less than 32 characters')
```

### Comparing `djsm-0.1.5/djsm.egg-info/PKG-INFO` & `djsm-0.1.51/djsm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.1.5
-Summary: Light weight module that allows you to store secrets encrypted in JSON and access them easily in your Django project.
+Version: 0.1.51
+Summary: Django package that allows you to store secrets encrypted in JSON and access them easily in your Django project.
 Author-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Maintainer-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
 Classifier: Programming Language :: Python :: 3
@@ -21,67 +21,38 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv>=0.19.2
 Requires-Dist: simple-file-handler>=0.0.1
 Requires-Dist: dcrypt>=0.0.1
 
-## DJSM - Django JSON Secrets Manager
+# DJSM - Django JSON Secrets Manager
 
-Light weight Python module that allows you to easily store and access your Django project's secrets like secret key, database password, etc., encrypted in a JSON file.
+Django package that allows you to easily store and access your Django project's secrets like secret key, database password, etc., encrypted in a JSON file.
 
 [View package on PyPI](https://pypi.org/project/djsm/)
 
 ## Installation and Quick Setup
 
 * Install the package using pip.
 
 ```bash
 pip install djsm
 ```
 
 * Setup or update a '.env' file for your project.
 
-Copy this into a .env file just outside your project (adjust as needed)
-
 ```.env
-DJSM_SECRETS_FILE_PATH = "./.secretfolder/path/secrets.json" 
+DJSM_SECRETS_FILE_PATH = "./.enc/path/secrets.json" 
 # Assign path to file you want secrets to be stored in. Even if it does not exist yet
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "secretkey"
 ```
 
-Your project structure should look like this:
-
-```bash
-|-- my_project
-|   |-- my_project
-|   |   |-- __init__.py
-|   |   |-- settings.py
-|   |   |-- urls.py
-|   |   |-- wsgi.py
-|   |
-|   |-- my_app
-|   |   |-- __init__.py
-|   |   |-- admin.py
-|   |   |-- apps.py
-|   |   |-- models.py
-|   |   |-- tests.py
-|   |   |-- views.py
-|   |
-|   |-- db.sqlite3
-|   |-- manage.py
-|   |-- .gitignore
-|   |-- requirements.txt
-|
-|-- venv
-|-- .env
-```
-
 * Import the package in your Django project
 
 In settings.py:
 
 ```python
 import djsm
 
@@ -94,22 +65,21 @@
 python manage.py runserver
 ```
 
 If everything was setup successfully, you should see "Setup OK!" on the terminal. Remember to remove the `djsm.check_setup()` line from your settings.py file.
 
 ## Usage
 
-Before starting, a '.env' file has to be created just outside the django project directory.
-In the file, the following should be added;
+Before starting, a '.env' file has to be created. In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
-SECRETS_FILE_PATH = "/.secrets/pathtofile/secrets.json"
+DJSM_SECRETS_FILE_PATH = "/.enc/pathtofile/secrets.json"
 ```
 
 * **`DJSM_SECRET_KEY_NAME`** -> Name with which the Django secret key should be stored.
 Example:
 
 ```.env
 DJSM_SECRET_KEY_NAME = 'django_secret_key'
@@ -262,15 +232,15 @@
 
 * `clean_up_and_reload()` -> Calls the `clean_up()` and `reload_env()` methods.
 
 ```python
 from djsm import DJSM  # DJSM is an alias for DjangoJSONSecretManager
 
 # Create a DJSM object
-secrets_manager = DJSM('./.secretfolder/secrets.json')
+secrets_manager = DJSM('./.enc/secrets.json')
 ```
 
 **DO NOT DELETE `cryptkeys.json` or any of the encryption keys. IF YOU DO, ALL ENCRYPTED SECRET WILL BE LOST**
 
 > NOTE: DJSM just provides an added layer of security in managing secrets in your application. It is not proven to be completely attack proof.
 
 Contributions are welcome. Please fork the repository and submit a pull request.
```

### Comparing `djsm-0.1.5/pyproject.toml` & `djsm-0.1.51/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 authors = [
   { name="Daniel T. Afolayan (ti-oluwa)", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="Daniel T. Afolayan (ti-oluwa)", email="tioluwa.dev@gmail.com" },
 ]
-description = "Light weight module that allows you to store secrets encrypted in JSON and access them easily in your Django project."
+description = "Django package that allows you to store secrets encrypted in JSON and access them easily in your Django project."
 keywords = [
     "Django", "Django Secrets Encryption"
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

