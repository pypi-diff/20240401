# Comparing `tmp/yandex-360-2.2.0.tar.gz` & `tmp/yandex-360-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandex-360-2.2.0.tar", last modified: Fri Mar 29 06:09:08 2024, max compression
+gzip compressed data, was "yandex-360-2.2.1.tar", last modified: Mon Apr  1 10:26:36 2024, max compression
```

## Comparing `yandex-360-2.2.0.tar` & `yandex-360-2.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.467116 yandex-360-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.463116 yandex-360-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-29 06:08:58.000000 yandex-360-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.463116 yandex-360-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-29 06:08:58.000000 yandex-360-2.2.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-29 06:08:58.000000 yandex-360-2.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-29 06:08:58.000000 yandex-360-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-29 06:08:58.000000 yandex-360-2.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-29 06:08:58.000000 yandex-360-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-29 06:09:08.467116 yandex-360-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-29 06:08:58.000000 yandex-360-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-29 06:08:58.000000 yandex-360-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.463116 yandex-360-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.463116 yandex-360-2.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.463116 yandex-360-2.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/_static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/lic.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-29 06:08:58.000000 yandex-360-2.2.0/docs/source/yandex_360.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-29 06:08:58.000000 yandex-360-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 06:09:08.467116 yandex-360-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-29 06:08:58.000000 yandex-360-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.467116 yandex-360-2.2.0/yandex_360/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 06:09:08.000000 yandex-360-2.2.0/yandex_360/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/a2fa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/antispam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/departments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)    20023 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19387 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/org.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/pwd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-03-29 06:08:58.000000 yandex-360-2.2.0/yandex_360/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:09:08.467116 yandex-360-2.2.0/yandex_360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-29 06:09:08.000000 yandex-360-2.2.0/yandex_360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-29 06:09:08.000000 yandex-360-2.2.0/yandex_360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 06:09:08.000000 yandex-360-2.2.0/yandex_360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 06:09:08.000000 yandex-360-2.2.0/yandex_360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 06:09:08.000000 yandex-360-2.2.0/yandex_360.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.460115 yandex-360-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.452115 yandex-360-2.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-01 10:26:31.000000 yandex-360-2.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.452115 yandex-360-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-01 10:26:31.000000 yandex-360-2.2.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-01 10:26:31.000000 yandex-360-2.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-01 10:26:31.000000 yandex-360-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-01 10:26:31.000000 yandex-360-2.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-01 10:26:31.000000 yandex-360-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 10:26:36.460115 yandex-360-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-01 10:26:31.000000 yandex-360-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-01 10:26:31.000000 yandex-360-2.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.456115 yandex-360-2.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.456115 yandex-360-2.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.456115 yandex-360-2.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/_static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/lic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-01 10:26:31.000000 yandex-360-2.2.1/docs/source/yandex_360.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-01 10:26:31.000000 yandex-360-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:26:36.460115 yandex-360-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 10:26:31.000000 yandex-360-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.456115 yandex-360-2.2.1/yandex_360/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 10:26:36.000000 yandex-360-2.2.1/yandex_360/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/a2fa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/antispam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/departments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20023 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19387 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20653 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-04-01 10:26:31.000000 yandex-360-2.2.1/yandex_360/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:36.460115 yandex-360-2.2.1/yandex_360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 10:26:36.000000 yandex-360-2.2.1/yandex_360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-01 10:26:36.000000 yandex-360-2.2.1/yandex_360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:26:36.000000 yandex-360-2.2.1/yandex_360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 10:26:36.000000 yandex-360-2.2.1/yandex_360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 10:26:36.000000 yandex-360-2.2.1/yandex_360.egg-info/top_level.txt
```

### Comparing `yandex-360-2.2.0/.github/workflows/codeql.yml` & `yandex-360-2.2.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/.github/workflows/python-publish.yml` & `yandex-360-2.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/.gitignore` & `yandex-360-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/.readthedocs.yaml` & `yandex-360-2.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/LICENSE` & `yandex-360-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/PKG-INFO` & `yandex-360-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-360
-Version: 2.2.0
+Version: 2.2.1
 Summary: Библиотека для Yandex 360 API
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/imercury13/yandex-360/issues
 Project-URL: Documentation, https://yandex-360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/yandex-360
 Keywords: yandex,yandex360,yandex-api,yandex360-api
```

### Comparing `yandex-360-2.2.0/docs/Makefile` & `yandex-360-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/docs/make.bat` & `yandex-360-2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/docs/source/conf.py` & `yandex-360-2.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/docs/source/glossary.rst` & `yandex-360-2.2.1/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/docs/source/index.rst` & `yandex-360-2.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/docs/source/lic.rst` & `yandex-360-2.2.1/docs/source/lic.rst`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/docs/source/usage.rst` & `yandex-360-2.2.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/docs/source/yandex_360.rst` & `yandex-360-2.2.1/docs/source/yandex_360.rst`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/pyproject.toml` & `yandex-360-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/a2fa.py` & `yandex-360-2.2.1/yandex_360/a2fa.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/antispam.py` & `yandex-360-2.2.1/yandex_360/antispam.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/auth.py` & `yandex-360-2.2.1/yandex_360/auth.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/departments.py` & `yandex-360-2.2.1/yandex_360/departments.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/dns.py` & `yandex-360-2.2.1/yandex_360/dns.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/domains.py` & `yandex-360-2.2.1/yandex_360/domains.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/groups.py` & `yandex-360-2.2.1/yandex_360/groups.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/logs.py` & `yandex-360-2.2.1/yandex_360/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Модуль для управления аудит-логов.
 """
 
+from urllib.parse import urlencode
 from jreq.jreq import safe_request
-import json
 
 def disk_log(token, orgID, pageSize=100, pageToken=None, beforeDate=None, afterDate=None, includeUids=None, excludeUids=None):
     """Функция возвращает список событий в аудит-логе Диска организации.
 
     :param token: :term:`Яндекс токен приложения`
     :type token: str
     :param orgID: :term:`ID организации в Яндекс 360`
@@ -16,17 +16,17 @@
     :param pageToken: Токен постраничной навигации
     :type pageToken: str
     :param beforeDate: Верхняя граница периода выборки в формате ISO 8601
     :type beforeDate: str
     :param afterDate: Нижняя граница периода выборки в формате ISO 8601
     :type afterDate: str
     :param includeUids: Список пользователей, действия которых должны быть включены в список событий
-    :type includeUids: str
+    :type includeUids: list
     :param excludeUids: Список пользователей, действия которых должны быть исключены из списка событий
-    :type excludeUids: str
+    :type excludeUids: list
     :return: :numref:`результат запроса %s <Результат запроса disk_log>`
     :rtype: dict
 
     .. code-block:: python
         :caption: Результат запроса disk_log
         :name: Результат запроса disk_log
 
@@ -54,19 +54,28 @@
             ],
             "nextPageToken": str
         }
 
     """
 
     url = f'https://api360.yandex.net/security/v1/org/{orgID}/audit_log/disk?pageSize={pageSize}'
-    if pageToken: url += f'&pageToken={pageToken}'
-    if beforeDate: url += f'&beforeDate={beforeDate}'
-    if afterDate: url += f'&afterDate={afterDate}'
-    if includeUids: url += f'&includeUids={includeUids}'
-    if excludeUids: url += f'&excludeUids={excludeUids}'
+    if pageToken:
+        url += f'&pageToken={pageToken}'
+    if beforeDate:
+        url += f'&beforeDate={beforeDate}'
+    if afterDate:
+        url += f'&afterDate={afterDate}'
+    if includeUids:
+        tmp = {"includeUids":includeUids}
+        tmp = urlencode(tmp, doseq=True)
+        url += f'&{tmp}'
+    if excludeUids:
+        tmp = {"excludeUids":excludeUids}
+        tmp = urlencode(tmp, doseq=True)
+        url += f'&{tmp}'
     headers={'Authorization': f'OAuth {token}', 'Content-type': 'application/json'}
 	
     return safe_request('get', url, headers)
 
 def mail_log(token, orgID, pageSize=100, pageToken=None, beforeDate=None, afterDate=None, includeUids=None, excludeUids=None, types=None):
     """Функция возвращает список событий в аудит-логе Почте организации.
 
@@ -79,19 +88,19 @@
     :param pageToken: Токен постраничной навигации
     :type pageToken: str
     :param beforeDate: Верхняя граница периода выборки в формате ISO 8601
     :type beforeDate: str
     :param afterDate: Нижняя граница периода выборки в формате ISO 8601
     :type afterDate: str
     :param includeUids: Список пользователей, действия которых должны быть включены в список событий
-    :type includeUids: str
+    :type includeUids: list
     :param excludeUids: Список пользователей, действия которых должны быть исключены из списка событий
-    :type excludeUids: str
+    :type excludeUids: list
     :param types: Типы событий которые должны быть включены в список. По умолчанию включаются все события
-    :type types: str
+    :type types: list
     :return: :numref:`результат запроса %s <Результат запроса mail_log>`
     :rtype: dict
 
     .. code-block:: python
         :caption: Результат запроса mail_log
         :name: Результат запроса mail_log
 
@@ -125,16 +134,28 @@
             ],
             "nextPageToken": str
         }
 
     """
 
     url = f'https://api360.yandex.net/security/v1/org/{orgID}/audit_log/mail?pageSize={pageSize}'
-    if pageToken: url += f'&pageToken={pageToken}'
-    if beforeDate: url += f'&beforeDate={beforeDate}'
-    if afterDate: url += f'&afterDate={afterDate}'
-    if includeUids: url += f'&includeUids={includeUids}'
-    if excludeUids: url += f'&excludeUids={excludeUids}'
-    if types: url += f'&types={types}'
+    if pageToken:
+        url += f'&pageToken={pageToken}'
+    if beforeDate:
+        url += f'&beforeDate={beforeDate}'
+    if afterDate:
+        url += f'&afterDate={afterDate}'
+    if includeUids:
+        tmp = {"includeUids":includeUids}
+        tmp = urlencode(tmp, doseq=True)
+        url += f'&{tmp}'
+    if excludeUids:
+        tmp = {"excludeUids":excludeUids}
+        tmp = urlencode(tmp, doseq=True)
+        url += f'&{tmp}'
+    if types:
+        tmp = {"types":types}
+        tmp = urlencode(tmp, doseq=True)
+        url += f'&{tmp}'
     headers={'Authorization': f'OAuth {token}', 'Content-type': 'application/json'}
 	
     return safe_request('get', url, headers)
```

### Comparing `yandex-360-2.2.0/yandex_360/mail.py` & `yandex-360-2.2.1/yandex_360/mail.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/org.py` & `yandex-360-2.2.1/yandex_360/org.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/pwd.py` & `yandex-360-2.2.1/yandex_360/pwd.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/routing.py` & `yandex-360-2.2.1/yandex_360/routing.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360/tools.py` & `yandex-360-2.2.1/yandex_360/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
     lst_dnss =[]
 
     dnss = dns.show_dns(token, orgID, domain)
     if check_request(dnss):
         while dnss['page'] <= dnss['pages']:
             lst_dnss += dnss['records']
-            dnss = dns.show_dns(token, orgID, domain, page=usrs['page']+1)
+            dnss = dns.show_dns(token, orgID, domain, page=dnss['page']+1)
         return {"records":lst_dnss,"page":dnss['page'],"pages":dnss['pages'],"perPage":dnss['perPage'],"total":dnss['total']}
     else:
         return dnss
 
 def get_orgs(token, orgID):
     """Функция возвращает список организаций пользователя
 
@@ -559,17 +559,17 @@
             "nextPageToken": str
         }
 
     """
 
     lst_mail =[]
 
-    mail = logs.mail_log(token, orgID, beforeDate=beforeDate, afterDate=afterDate, includeUids=includeUids, excludeUids=excludeUids, types=None)
+    mail = logs.mail_log(token, orgID, beforeDate=beforeDate, afterDate=afterDate, includeUids=includeUids, excludeUids=excludeUids, types=types)
     if check_request(mail):
         lst_mail += mail['events']
-        mail = logs.mail_log(token, orgID, pageToken=mail['nextPageToken'], beforeDate=beforeDate, afterDate=afterDate, includeUids=includeUids, excludeUids=excludeUids, types=None)
+        mail = logs.mail_log(token, orgID, pageToken=mail['nextPageToken'], beforeDate=beforeDate, afterDate=afterDate, includeUids=includeUids, excludeUids=excludeUids, types=types)
         while mail['nextPageToken'] != '':
             lst_mail += mail['events']
-            mail = logs.mail_log(token, orgID, pageToken=mail['nextPageToken'], beforeDate=beforeDate, afterDate=afterDate, includeUids=includeUids, excludeUids=excludeUids, types=None)
+            mail = logs.mail_log(token, orgID, pageToken=mail['nextPageToken'], beforeDate=beforeDate, afterDate=afterDate, includeUids=includeUids, excludeUids=excludeUids, types=types)
         return {"events":lst_mail,"nextPageToken":mail['nextPageToken']}
     else:
         return mail
```

### Comparing `yandex-360-2.2.0/yandex_360/users.py` & `yandex-360-2.2.1/yandex_360/users.py`

 * *Files identical despite different names*

### Comparing `yandex-360-2.2.0/yandex_360.egg-info/PKG-INFO` & `yandex-360-2.2.1/yandex_360.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-360
-Version: 2.2.0
+Version: 2.2.1
 Summary: Библиотека для Yandex 360 API
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/imercury13/yandex-360/issues
 Project-URL: Documentation, https://yandex-360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/yandex-360
 Keywords: yandex,yandex360,yandex-api,yandex360-api
```

### Comparing `yandex-360-2.2.0/yandex_360.egg-info/SOURCES.txt` & `yandex-360-2.2.1/yandex_360.egg-info/SOURCES.txt`

 * *Files identical despite different names*

