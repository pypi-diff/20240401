# Comparing `tmp/sddl-0.3.0.tar.gz` & `tmp/sddl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddl-0.3.0.tar", max compression
+gzip compressed data, was "sddl-0.3.1.tar", max compression
```

## Comparing `sddl-0.3.0.tar` & `sddl-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     3186 2023-09-20 07:47:28.168695 sddl-0.3.0/README.md
--rw-r--r--   0        0        0      412 2023-09-20 08:22:47.653949 sddl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1657 2023-09-20 08:23:39.526067 sddl-0.3.0/sddl/__main__.py
--rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 sddl-0.3.0/setup.py
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 sddl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3186 2024-04-01 20:12:49.513148 sddl-0.3.1/README.md
+-rw-r--r--   0        0        0      412 2024-04-01 20:12:49.513148 sddl-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1657 2024-04-01 20:12:49.513148 sddl-0.3.1/sddl/__main__.py
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 sddl-0.3.1/PKG-INFO
```

### Comparing `sddl-0.3.0/README.md` & `sddl-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sddl-0.3.0/sddl/__main__.py` & `sddl-0.3.1/sddl/__main__.py`

 * *Files identical despite different names*

### Comparing `sddl-0.3.0/setup.py` & `sddl-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,63 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sddl
+Version: 0.3.1
+Summary: CLI frontend for sddl-parser
+Author: Max Harley
+Author-email: maxh@maxh.io
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: sddl-parser (>=0.5.0,<0.6.0)
+Description-Content-Type: text/markdown
+
+# SDDL
+
+## Usage
+
+```bash
+$ sddl -h
+usage: sddl [-h] [--type TYPE] [--list-types] [--json] [sddl]
+
+Read SDDL strings
+
+positional arguments:
+  sddl          SDDL string to parse. If not provided, read from stdin.
+
+options:
+  -h, --help    show this help message and exit
+  --type TYPE   Type of ACE to parse. Default: GenericAccessRights
+  --list-types  List available ACE types
+  --json        Output as JSON
+
+Example: `sddl 'O:BAG:BAD:(A;;GA;;;WD)'` or `echo 'O:BAG:BAD:(A;;GA;;;WD)' | sddl`
+```
+
+## Examples
+
+- Using an alternative rights type
+
+```bash
+sddl 'O:SYG:SYD:AI(A;ID;FA;;;SY)(A;ID;FA;;;BA)(A;ID;0x1200a9;;;BU)(A;ID;0x1200a9;;;AC)(A;ID;0x1200a9;;;
+S-1-15-2-2)' --type RegistryKeyAccessRights
+Owner: LOCAL_SYSTEM
+Group: LOCAL_SYSTEM
+DACL:
+  SDDL_AUTO_INHERITED
+    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|KEY_SET_VALUE|KEY_WOW64_64KEY|KEY_CREATE_SUB_KEY|DELETE|READ_CONTROL|WRITE_DAC|KEY_ENUMERATE_SUB_KEYS|WRITE_OWNER|SYNCHRONIZE|KEY_WRITE|KEY_NOTIFY|KEY_READ|KEY_ALL_ACCESS LOCAL_SYSTEM
+    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|KEY_SET_VALUE|KEY_WOW64_64KEY|KEY_CREATE_SUB_KEY|DELETE|READ_CONTROL|WRITE_DAC|KEY_ENUMERATE_SUB_KEYS|WRITE_OWNER|SYNCHRONIZE|KEY_WRITE|KEY_NOTIFY|KEY_READ|KEY_ALL_ACCESS BUILTIN_ADMINISTRATORS
+    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|READ_CONTROL|SYNCHRONIZE|KEY_ENUMERATE_SUB_KEYS BUILTIN_USERS
+    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|READ_CONTROL|SYNCHRONIZE|KEY_ENUMERATE_SUB_KEYS ALL_APP_PACKAGES
+    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|READ_CONTROL|SYNCHRONIZE|KEY_ENUMERATE_SUB_KEYS S-1-15-2-2
+SACL:
+```
+
+- Output to JSON
+
+```bash
+$ sddl 'O:SYG:SYD:AI(A;ID;FA;;;SY)(A;ID;FA;;;BA)(A;ID;0x1200a9;;;BU)(A;ID;0x1200a9;;;AC)(A;ID;0x1200a9;;;
+S-1-15-2-2)' --type RegistryKeyAccessRights --json
+{"owner": "LOCAL_SYSTEM", "group": "LOCAL_SYSTEM", "dacl": {"flags": ["SDDL_AUTO_INHERITED"], "aces": [{"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "KEY_SET_VALUE", "KEY_WOW64_64KEY", "KEY_CREATE_SUB_KEY", "DELETE", "READ_CONTROL", "WRITE_DAC", "KEY_ENUMERATE_SUB_KEYS", "WRITE_OWNER", "SYNCHRONIZE", "KEY_WRITE", "KEY_NOTIFY", "KEY_READ", "KEY_ALL_ACCESS"], "sid": "LOCAL_SYSTEM"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "KEY_SET_VALUE", "KEY_WOW64_64KEY", "KEY_CREATE_SUB_KEY", "DELETE", "READ_CONTROL", "WRITE_DAC", "KEY_ENUMERATE_SUB_KEYS", "WRITE_OWNER", "SYNCHRONIZE", "KEY_WRITE", "KEY_NOTIFY", "KEY_READ", "KEY_ALL_ACCESS"], "sid": "BUILTIN_ADMINISTRATORS"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "READ_CONTROL", "SYNCHRONIZE", "KEY_ENUMERATE_SUB_KEYS"], "sid": "BUILTIN_USERS"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "READ_CONTROL", "SYNCHRONIZE", "KEY_ENUMERATE_SUB_KEYS"], "sid": "ALL_APP_PACKAGES"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "READ_CONTROL", "SYNCHRONIZE", "KEY_ENUMERATE_SUB_KEYS"], "sid": "S-1-15-2-2"}]}, "sacl": null}
+```
 
-packages = \
-['sddl']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['sddl-parser>=0.5.0,<0.6.0']
-
-entry_points = \
-{'console_scripts': ['sddl = sddl.__main__:main']}
-
-setup_kwargs = {
-    'name': 'sddl',
-    'version': '0.3.0',
-    'description': 'CLI frontend for sddl-parser',
-    'long_description': '# SDDL\n\n## Usage\n\n```bash\n$ sddl -h\nusage: sddl [-h] [--type TYPE] [--list-types] [--json] [sddl]\n\nRead SDDL strings\n\npositional arguments:\n  sddl          SDDL string to parse. If not provided, read from stdin.\n\noptions:\n  -h, --help    show this help message and exit\n  --type TYPE   Type of ACE to parse. Default: GenericAccessRights\n  --list-types  List available ACE types\n  --json        Output as JSON\n\nExample: `sddl \'O:BAG:BAD:(A;;GA;;;WD)\'` or `echo \'O:BAG:BAD:(A;;GA;;;WD)\' | sddl`\n```\n\n## Examples\n\n- Using an alternative rights type\n\n```bash\nsddl \'O:SYG:SYD:AI(A;ID;FA;;;SY)(A;ID;FA;;;BA)(A;ID;0x1200a9;;;BU)(A;ID;0x1200a9;;;AC)(A;ID;0x1200a9;;;\nS-1-15-2-2)\' --type RegistryKeyAccessRights\nOwner: LOCAL_SYSTEM\nGroup: LOCAL_SYSTEM\nDACL:\n  SDDL_AUTO_INHERITED\n    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|KEY_SET_VALUE|KEY_WOW64_64KEY|KEY_CREATE_SUB_KEY|DELETE|READ_CONTROL|WRITE_DAC|KEY_ENUMERATE_SUB_KEYS|WRITE_OWNER|SYNCHRONIZE|KEY_WRITE|KEY_NOTIFY|KEY_READ|KEY_ALL_ACCESS LOCAL_SYSTEM\n    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|KEY_SET_VALUE|KEY_WOW64_64KEY|KEY_CREATE_SUB_KEY|DELETE|READ_CONTROL|WRITE_DAC|KEY_ENUMERATE_SUB_KEYS|WRITE_OWNER|SYNCHRONIZE|KEY_WRITE|KEY_NOTIFY|KEY_READ|KEY_ALL_ACCESS BUILTIN_ADMINISTRATORS\n    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|READ_CONTROL|SYNCHRONIZE|KEY_ENUMERATE_SUB_KEYS BUILTIN_USERS\n    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|READ_CONTROL|SYNCHRONIZE|KEY_ENUMERATE_SUB_KEYS ALL_APP_PACKAGES\n    ACCESS_ALLOWED INHERITED KEY_CREATE_LINK|KEY_QUERY_VALUE|READ_CONTROL|SYNCHRONIZE|KEY_ENUMERATE_SUB_KEYS S-1-15-2-2\nSACL:\n```\n\n- Output to JSON\n\n```bash\n$ sddl \'O:SYG:SYD:AI(A;ID;FA;;;SY)(A;ID;FA;;;BA)(A;ID;0x1200a9;;;BU)(A;ID;0x1200a9;;;AC)(A;ID;0x1200a9;;;\nS-1-15-2-2)\' --type RegistryKeyAccessRights --json\n{"owner": "LOCAL_SYSTEM", "group": "LOCAL_SYSTEM", "dacl": {"flags": ["SDDL_AUTO_INHERITED"], "aces": [{"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "KEY_SET_VALUE", "KEY_WOW64_64KEY", "KEY_CREATE_SUB_KEY", "DELETE", "READ_CONTROL", "WRITE_DAC", "KEY_ENUMERATE_SUB_KEYS", "WRITE_OWNER", "SYNCHRONIZE", "KEY_WRITE", "KEY_NOTIFY", "KEY_READ", "KEY_ALL_ACCESS"], "sid": "LOCAL_SYSTEM"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "KEY_SET_VALUE", "KEY_WOW64_64KEY", "KEY_CREATE_SUB_KEY", "DELETE", "READ_CONTROL", "WRITE_DAC", "KEY_ENUMERATE_SUB_KEYS", "WRITE_OWNER", "SYNCHRONIZE", "KEY_WRITE", "KEY_NOTIFY", "KEY_READ", "KEY_ALL_ACCESS"], "sid": "BUILTIN_ADMINISTRATORS"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "READ_CONTROL", "SYNCHRONIZE", "KEY_ENUMERATE_SUB_KEYS"], "sid": "BUILTIN_USERS"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "READ_CONTROL", "SYNCHRONIZE", "KEY_ENUMERATE_SUB_KEYS"], "sid": "ALL_APP_PACKAGES"}, {"type": "ACCESS_ALLOWED", "flags": ["INHERITED"], "rights": ["KEY_CREATE_LINK", "KEY_QUERY_VALUE", "READ_CONTROL", "SYNCHRONIZE", "KEY_ENUMERATE_SUB_KEYS"], "sid": "S-1-15-2-2"}]}, "sacl": null}\n```\n',
-    'author': 'Max Harley',
-    'author_email': 'maxh@maxh.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

