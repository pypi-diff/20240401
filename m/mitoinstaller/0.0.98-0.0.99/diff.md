# Comparing `tmp/mitoinstaller-0.0.98.tar.gz` & `tmp/mitoinstaller-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitoinstaller-0.0.98.tar", last modified: Thu Jan 27 18:39:49 2022, max compression
+gzip compressed data, was "mitoinstaller-0.0.99.tar", last modified: Thu Jan 27 18:41:06 2022, max compression
```

## Comparing `mitoinstaller-0.0.98.tar` & `mitoinstaller-0.0.99.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:39:49.331659 mitoinstaller-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-01-27 18:39:49.331659 mitoinstaller-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:39:49.327659 mitoinstaller-0.0.98/mitoinstaller/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-27 18:39:43.000000 mitoinstaller-0.0.98/mitoinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7290 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/create_startup_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/do_upgrade_to_jupyterlab_3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:39:49.327659 mitoinstaller-0.0.98/mitoinstaller/installer_steps/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/installer_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/installer_steps/final_installer_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/installer_steps/initial_installer_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/installer_steps/installer_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/installer_steps/installer_step_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/installer_steps/mitosheet3_installer_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/installer_steps/mitosheet_installer_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/starter_notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/mitoinstaller/user_install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:39:49.327659 mitoinstaller-0.0.98/mitoinstaller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-01-27 18:39:49.000000 mitoinstaller-0.0.98/mitoinstaller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-01-27 18:39:49.000000 mitoinstaller-0.0.98/mitoinstaller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 18:39:49.000000 mitoinstaller-0.0.98/mitoinstaller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-01-27 18:39:49.000000 mitoinstaller-0.0.98/mitoinstaller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-27 18:39:49.000000 mitoinstaller-0.0.98/mitoinstaller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-27 18:39:49.331659 mitoinstaller-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:39:49.331659 mitoinstaller-0.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4243 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/tests/test_do_upgrade_to_jupyterlab_3.py
--rw-r--r--   0 runner    (1001) docker     (121)     5477 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/tests/test_installs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/tests/test_static_user_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-01-27 18:39:33.000000 mitoinstaller-0.0.98/tests/test_upgrades.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:41:06.098668 mitoinstaller-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-01-27 18:41:06.098668 mitoinstaller-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:41:06.094668 mitoinstaller-0.0.99/mitoinstaller/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-27 18:41:01.000000 mitoinstaller-0.0.99/mitoinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7290 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/create_startup_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/do_upgrade_to_jupyterlab_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/install.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:41:06.098668 mitoinstaller-0.0.99/mitoinstaller/installer_steps/
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/installer_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/installer_steps/final_installer_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/installer_steps/initial_installer_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/installer_steps/installer_step.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/installer_steps/installer_step_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/installer_steps/mitosheet3_installer_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/installer_steps/mitosheet_installer_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/starter_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/mitoinstaller/user_install.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:41:06.094668 mitoinstaller-0.0.99/mitoinstaller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-01-27 18:41:05.000000 mitoinstaller-0.0.99/mitoinstaller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-01-27 18:41:05.000000 mitoinstaller-0.0.99/mitoinstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 18:41:05.000000 mitoinstaller-0.0.99/mitoinstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-01-27 18:41:05.000000 mitoinstaller-0.0.99/mitoinstaller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-27 18:41:05.000000 mitoinstaller-0.0.99/mitoinstaller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-27 18:41:06.098668 mitoinstaller-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 18:41:06.098668 mitoinstaller-0.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4243 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/tests/test_do_upgrade_to_jupyterlab_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5477 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/tests/test_installs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/tests/test_static_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-01-27 18:40:55.000000 mitoinstaller-0.0.99/tests/test_upgrades.py
```

### Comparing `mitoinstaller-0.0.98/README.md` & `mitoinstaller-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/__main__.py` & `mitoinstaller-0.0.99/mitoinstaller/__main__.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/commands.py` & `mitoinstaller-0.0.99/mitoinstaller/commands.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/create_startup_file.py` & `mitoinstaller-0.0.99/mitoinstaller/create_startup_file.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/do_upgrade_to_jupyterlab_3.py` & `mitoinstaller-0.0.99/mitoinstaller/do_upgrade_to_jupyterlab_3.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/install.py` & `mitoinstaller-0.0.99/mitoinstaller/install.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/installer_steps/final_installer_steps.py` & `mitoinstaller-0.0.99/mitoinstaller/installer_steps/final_installer_steps.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/installer_steps/initial_installer_steps.py` & `mitoinstaller-0.0.99/mitoinstaller/installer_steps/initial_installer_steps.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/installer_steps/installer_step.py` & `mitoinstaller-0.0.99/mitoinstaller/installer_steps/installer_step.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/installer_steps/installer_step_utils.py` & `mitoinstaller-0.0.99/mitoinstaller/installer_steps/installer_step_utils.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/installer_steps/mitosheet3_installer_steps.py` & `mitoinstaller-0.0.99/mitoinstaller/installer_steps/mitosheet3_installer_steps.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/installer_steps/mitosheet_installer_steps.py` & `mitoinstaller-0.0.99/mitoinstaller/installer_steps/mitosheet_installer_steps.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/log_utils.py` & `mitoinstaller-0.0.99/mitoinstaller/log_utils.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/starter_notebook.py` & `mitoinstaller-0.0.99/mitoinstaller/starter_notebook.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller/user_install.py` & `mitoinstaller-0.0.99/mitoinstaller/user_install.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/mitoinstaller.egg-info/SOURCES.txt` & `mitoinstaller-0.0.99/mitoinstaller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/setup.py` & `mitoinstaller-0.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/tests/conftest.py` & `mitoinstaller-0.0.99/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/tests/test_do_upgrade_to_jupyterlab_3.py` & `mitoinstaller-0.0.99/tests/test_do_upgrade_to_jupyterlab_3.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/tests/test_installs.py` & `mitoinstaller-0.0.99/tests/test_installs.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/tests/test_static_user_id.py` & `mitoinstaller-0.0.99/tests/test_static_user_id.py`

 * *Files identical despite different names*

### Comparing `mitoinstaller-0.0.98/tests/test_upgrades.py` & `mitoinstaller-0.0.99/tests/test_upgrades.py`

 * *Files identical despite different names*

