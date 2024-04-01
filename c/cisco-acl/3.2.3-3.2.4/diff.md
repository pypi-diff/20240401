# Comparing `tmp/cisco_acl-3.2.3.tar.gz` & `tmp/cisco_acl-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cisco_acl-3.2.3.tar", max compression
+gzip compressed data, was "cisco_acl-3.2.4.tar", max compression
```

## Comparing `cisco_acl-3.2.3.tar` & `cisco_acl-3.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      933 2023-12-04 09:59:54.578612 cisco_acl-3.2.3/cisco_acl/__init__.py
--rw-r--r--   0        0        0    23463 2024-02-01 07:26:36.102829 cisco_acl-3.2.3/cisco_acl/ace.py
--rw-r--r--   0        0        0     4934 2024-02-01 07:26:36.103829 cisco_acl-3.2.3/cisco_acl/ace_base.py
--rw-r--r--   0        0        0    15869 2024-01-31 19:23:54.895813 cisco_acl-3.2.3/cisco_acl/ace_group.py
--rw-r--r--   0        0        0    23638 2024-02-01 07:26:36.103829 cisco_acl-3.2.3/cisco_acl/acl.py
--rw-r--r--   0        0        0    13568 2023-11-22 14:09:38.045056 cisco_acl-3.2.3/cisco_acl/addr_group.py
--rw-r--r--   0        0        0     4799 2023-12-04 10:03:35.657539 cisco_acl-3.2.3/cisco_acl/address.py
--rw-r--r--   0        0        0    11334 2024-02-01 07:26:36.104829 cisco_acl-3.2.3/cisco_acl/address_ag.py
--rw-r--r--   0        0        0    20668 2024-02-01 07:26:36.105830 cisco_acl-3.2.3/cisco_acl/address_base.py
--rw-r--r--   0        0        0     3484 2024-02-01 07:26:36.106829 cisco_acl-3.2.3/cisco_acl/base.py
--rw-r--r--   0        0        0    15308 2023-12-04 10:03:35.659142 cisco_acl-3.2.3/cisco_acl/config_parser.py
--rw-r--r--   0        0        0    14905 2024-02-01 07:26:36.107829 cisco_acl-3.2.3/cisco_acl/functions.py
--rw-r--r--   0        0        0     3703 2023-11-22 14:09:38.048586 cisco_acl-3.2.3/cisco_acl/group.py
--rw-r--r--   0        0        0    16498 2024-02-01 07:26:36.108828 cisco_acl-3.2.3/cisco_acl/helpers.py
--rw-r--r--   0        0        0     3315 2024-02-01 08:31:19.860713 cisco_acl-3.2.3/cisco_acl/option.py
--rw-r--r--   0        0        0     5587 2024-02-01 07:26:36.108828 cisco_acl-3.2.3/cisco_acl/parsers.py
--rw-r--r--   0        0        0    12357 2024-02-01 07:26:36.109829 cisco_acl-3.2.3/cisco_acl/port.py
--rw-r--r--   0        0        0     8446 2023-12-04 10:03:35.655538 cisco_acl-3.2.3/cisco_acl/port_name.py
--rw-r--r--   0        0        0     7454 2024-02-01 07:26:36.110829 cisco_acl-3.2.3/cisco_acl/protocol.py
--rw-r--r--   0        0        0        0 2022-10-06 06:10:23.243000 cisco_acl-3.2.3/cisco_acl/py.typed
--rw-r--r--   0        0        0     3628 2023-11-22 14:09:38.048586 cisco_acl-3.2.3/cisco_acl/remark.py
--rw-r--r--   0        0        0     1111 2023-11-22 14:09:38.048586 cisco_acl-3.2.3/cisco_acl/types_.py
--rw-r--r--   0        0        0    12460 2024-02-01 07:26:36.111827 cisco_acl-3.2.3/cisco_acl/wildcard.py
--rw-r--r--   0        0        0     2553 2024-02-01 08:47:29.118895 cisco_acl-3.2.3/pyproject.toml
--rw-r--r--   0        0        0     8331 2024-02-01 08:47:29.132897 cisco_acl-3.2.3/README.rst
--rw-r--r--   0        0        0     9308 1970-01-01 00:00:00.000000 cisco_acl-3.2.3/PKG-INFO
+-rw-r--r--   0        0        0      933 2023-12-04 09:59:54.578612 cisco_acl-3.2.4/cisco_acl/__init__.py
+-rw-r--r--   0        0        0    23463 2024-02-01 07:26:36.102829 cisco_acl-3.2.4/cisco_acl/ace.py
+-rw-r--r--   0        0        0     4934 2024-02-01 07:26:36.103829 cisco_acl-3.2.4/cisco_acl/ace_base.py
+-rw-r--r--   0        0        0    15869 2024-01-31 19:23:54.895813 cisco_acl-3.2.4/cisco_acl/ace_group.py
+-rw-r--r--   0        0        0    23734 2024-04-01 13:58:58.121802 cisco_acl-3.2.4/cisco_acl/acl.py
+-rw-r--r--   0        0        0    13568 2023-11-22 14:09:38.045056 cisco_acl-3.2.4/cisco_acl/addr_group.py
+-rw-r--r--   0        0        0     4799 2023-12-04 10:03:35.657539 cisco_acl-3.2.4/cisco_acl/address.py
+-rw-r--r--   0        0        0    11334 2024-02-01 07:26:36.104829 cisco_acl-3.2.4/cisco_acl/address_ag.py
+-rw-r--r--   0        0        0    20668 2024-02-01 07:26:36.105830 cisco_acl-3.2.4/cisco_acl/address_base.py
+-rw-r--r--   0        0        0     3484 2024-02-01 07:26:36.106829 cisco_acl-3.2.4/cisco_acl/base.py
+-rw-r--r--   0        0        0    15308 2023-12-04 10:03:35.659142 cisco_acl-3.2.4/cisco_acl/config_parser.py
+-rw-r--r--   0        0        0    14905 2024-02-01 07:26:36.107829 cisco_acl-3.2.4/cisco_acl/functions.py
+-rw-r--r--   0        0        0     3703 2023-11-22 14:09:38.048586 cisco_acl-3.2.4/cisco_acl/group.py
+-rw-r--r--   0        0        0    16498 2024-02-01 07:26:36.108828 cisco_acl-3.2.4/cisco_acl/helpers.py
+-rw-r--r--   0        0        0     3315 2024-02-01 08:51:52.953706 cisco_acl-3.2.4/cisco_acl/option.py
+-rw-r--r--   0        0        0     5587 2024-02-01 07:26:36.108828 cisco_acl-3.2.4/cisco_acl/parsers.py
+-rw-r--r--   0        0        0    12357 2024-02-01 07:26:36.109829 cisco_acl-3.2.4/cisco_acl/port.py
+-rw-r--r--   0        0        0     8446 2023-12-04 10:03:35.655538 cisco_acl-3.2.4/cisco_acl/port_name.py
+-rw-r--r--   0        0        0     7454 2024-02-01 07:26:36.110829 cisco_acl-3.2.4/cisco_acl/protocol.py
+-rw-r--r--   0        0        0        0 2022-10-06 06:10:23.243000 cisco_acl-3.2.4/cisco_acl/py.typed
+-rw-r--r--   0        0        0     3628 2023-11-22 14:09:38.048586 cisco_acl-3.2.4/cisco_acl/remark.py
+-rw-r--r--   0        0        0     1111 2023-11-22 14:09:38.048586 cisco_acl-3.2.4/cisco_acl/types_.py
+-rw-r--r--   0        0        0    12460 2024-02-01 07:26:36.111827 cisco_acl-3.2.4/cisco_acl/wildcard.py
+-rw-r--r--   0        0        0     2553 2024-04-01 13:58:58.123806 cisco_acl-3.2.4/pyproject.toml
+-rw-r--r--   0        0        0     8331 2024-04-01 13:58:58.119804 cisco_acl-3.2.4/README.rst
+-rw-r--r--   0        0        0     9308 1970-01-01 00:00:00.000000 cisco_acl-3.2.4/PKG-INFO
```

### Comparing `cisco_acl-3.2.3/cisco_acl/__init__.py` & `cisco_acl-3.2.4/cisco_acl/__init__.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/ace.py` & `cisco_acl-3.2.4/cisco_acl/ace.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/ace_base.py` & `cisco_acl-3.2.4/cisco_acl/ace_base.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/ace_group.py` & `cisco_acl-3.2.4/cisco_acl/ace_group.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/acl.py` & `cisco_acl-3.2.4/cisco_acl/acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,17 @@
         grouped_items_d: Dict[str, LUAceg] = {}
         group_name = ""
         grouped_items_d[group_name] = []
         for item in ungrouped_l:
             if isinstance(item, Remark):
                 if item.text.startswith(group_by):
                     group_name = item.text
-                    grouped_items_d[group_name] = []
+                    if item.text not in grouped_items_d:
+                        grouped_items_d[group_name] = [item]
+                    continue
             grouped_items_d[group_name].append(item)
 
         grouped_items: LUAceg = []
         for group_name, aces_items in grouped_items_d.items():
             if aces_items:
                 aceg_o = AceGroup(
                     platform=self._platform,
```

### Comparing `cisco_acl-3.2.3/cisco_acl/addr_group.py` & `cisco_acl-3.2.4/cisco_acl/addr_group.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/address.py` & `cisco_acl-3.2.4/cisco_acl/address.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/address_ag.py` & `cisco_acl-3.2.4/cisco_acl/address_ag.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/address_base.py` & `cisco_acl-3.2.4/cisco_acl/address_base.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/base.py` & `cisco_acl-3.2.4/cisco_acl/base.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/config_parser.py` & `cisco_acl-3.2.4/cisco_acl/config_parser.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/functions.py` & `cisco_acl-3.2.4/cisco_acl/functions.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/group.py` & `cisco_acl-3.2.4/cisco_acl/group.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/helpers.py` & `cisco_acl-3.2.4/cisco_acl/helpers.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/option.py` & `cisco_acl-3.2.4/cisco_acl/option.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/parsers.py` & `cisco_acl-3.2.4/cisco_acl/parsers.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/port.py` & `cisco_acl-3.2.4/cisco_acl/port.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/port_name.py` & `cisco_acl-3.2.4/cisco_acl/port_name.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/protocol.py` & `cisco_acl-3.2.4/cisco_acl/protocol.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/remark.py` & `cisco_acl-3.2.4/cisco_acl/remark.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/types_.py` & `cisco_acl-3.2.4/cisco_acl/types_.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/cisco_acl/wildcard.py` & `cisco_acl-3.2.4/cisco_acl/wildcard.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.3/pyproject.toml` & `cisco_acl-3.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cisco_acl"
-version = "3.2.3"
+version = "3.2.4"
 description = "Python package to parse and manage Cisco ACL (Access Control List)"
 authors = ["Vladimirs Prusakovs <vladimir.prusakovs@gmail.com>"]
 readme = "README.rst"
 license = "Apache-2.0"
 homepage = "https://github.com/vladimirs-git/cisco-acl"
 repository = "https://github.com/vladimirs-git/cisco-acl"
 keywords = ["cisco", "acl", "ios", "nexus", "nx-os"]
@@ -36,15 +36,15 @@
 vhelpers = "^0.1.14"
 
 [tool.poetry.extras]
 test = ["pytest"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/vladimirs-git/cisco-acl/issues"
-"Download URL" = "https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.3.tar.gz"
+"Download URL" = "https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz"
 
 [tool.pylint]
 max-line-length = 100
 
 [tool.pylint.message_control]
 max-args = 10
 max-attributes = 13
```

### Comparing `cisco_acl-3.2.3/README.rst` & `cisco_acl-3.2.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     pip install cisco-acl
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.3.tar.gz
+    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/cisco-acl
```

### Comparing `cisco_acl-3.2.3/PKG-INFO` & `cisco_acl-3.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cisco_acl
-Version: 3.2.3
+Version: 3.2.4
 Summary: Python package to parse and manage Cisco ACL (Access Control List)
 Home-page: https://github.com/vladimirs-git/cisco-acl
 License: Apache-2.0
 Keywords: cisco,acl,ios,nexus,nx-os
 Author: Vladimirs Prusakovs
 Author-email: vladimir.prusakovs@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Provides-Extra: test
 Requires-Dist: netports (>=0.12.1,<0.13.0)
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/cisco-acl/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.3.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz
 Project-URL: Repository, https://github.com/vladimirs-git/cisco-acl
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://img.shields.io/pypi/v/cisco-acl.svg
    :target: https://pypi.python.org/pypi/cisco-acl
 .. image:: https://img.shields.io/pypi/pyversions/cisco-acl.svg
@@ -83,15 +83,15 @@
 
     pip install cisco-acl
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.3.tar.gz
+    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/cisco-acl
```

