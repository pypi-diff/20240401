# Comparing `tmp/eth-typing-4.0.0.tar.gz` & `tmp/eth-typing-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-typing-4.0.0.tar", last modified: Tue Jan  9 22:04:37 2024, max compression
+gzip compressed data, was "eth-typing-4.1.0.tar", last modified: Mon Apr  1 19:28:09 2024, max compression
```

## Comparing `eth-typing-4.0.0.tar` & `eth-typing-4.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-09 22:04:37.849373 eth-typing-4.0.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2023-04-25 16:25:20.000000 eth-typing-4.0.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-01-09 21:37:13.000000 eth-typing-4.0.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4954 2024-01-09 22:04:37.849373 eth-typing-4.0.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3285 2024-01-09 21:37:13.000000 eth-typing-4.0.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-09 22:04:37.849373 eth-typing-4.0.0/eth_typing/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      952 2024-01-09 21:37:13.000000 eth-typing-4.0.0/eth_typing/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       85 2023-04-13 15:36:53.000000 eth-typing-4.0.0/eth_typing/abi.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      191 2023-04-25 16:25:20.000000 eth-typing-4.0.0/eth_typing/bls.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       71 2023-04-13 15:36:53.000000 eth-typing-4.0.0/eth_typing/discovery.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      117 2023-04-25 16:25:20.000000 eth-typing-4.0.0/eth_typing/encoding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      458 2024-01-09 21:37:13.000000 eth-typing-4.0.0/eth_typing/enums.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      173 2023-04-25 16:25:20.000000 eth-typing-4.0.0/eth_typing/ethpm.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      546 2024-01-09 21:37:13.000000 eth-typing-4.0.0/eth_typing/evm.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    20845 2024-01-09 21:37:13.000000 eth-typing-4.0.0/eth_typing/networks.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-13 15:36:53.000000 eth-typing-4.0.0/eth_typing/py.typed
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-09 22:04:37.849373 eth-typing-4.0.0/eth_typing.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4954 2024-01-09 22:04:37.000000 eth-typing-4.0.0/eth_typing.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      488 2024-01-09 22:04:37.000000 eth-typing-4.0.0/eth_typing.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-01-09 22:04:37.000000 eth-typing-4.0.0/eth_typing.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-04-13 17:58:42.000000 eth-typing-4.0.0/eth_typing.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      284 2024-01-09 22:04:37.000000 eth-typing-4.0.0/eth_typing.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       11 2024-01-09 22:04:37.000000 eth-typing-4.0.0/eth_typing.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3425 2024-01-09 22:02:05.000000 eth-typing-4.0.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-01-09 22:04:37.849373 eth-typing-4.0.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1894 2024-01-09 22:03:53.000000 eth-typing-4.0.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-09 22:04:37.845373 eth-typing-4.0.0/tests/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-01-09 22:04:37.849373 eth-typing-4.0.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       93 2024-01-09 22:02:05.000000 eth-typing-4.0.0/tests/core/test_import.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.088426 eth-typing-4.1.0/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2024-03-25 21:51:21.000000 eth-typing-4.1.0/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-03-25 21:51:21.000000 eth-typing-4.1.0/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5005 2024-04-01 19:28:09.088426 eth-typing-4.1.0/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3285 2024-03-25 21:51:21.000000 eth-typing-4.1.0/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/eth_typing/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      952 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       85 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/abi.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      191 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/bls.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       71 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/discovery.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      117 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      458 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/enums.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      173 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/ethpm.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      546 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/evm.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    20845 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/networks.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/py.typed
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/eth_typing.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5005 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      500 2024-04-01 19:28:09.000000 eth-typing-4.1.0/eth_typing.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      284 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       11 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3459 2024-04-01 18:23:03.000000 eth-typing-4.1.0/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-01 19:28:09.088426 eth-typing-4.1.0/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1944 2024-04-01 19:27:50.000000 eth-typing-4.1.0/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      105 2024-03-25 21:51:21.000000 eth-typing-4.1.0/tests/core/test_import_and_version.py
```

### Comparing `eth-typing-4.0.0/LICENSE` & `eth-typing-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-typing-4.0.0/PKG-INFO` & `eth-typing-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 4.0.0
+Version: 4.1.0
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
```

### Comparing `eth-typing-4.0.0/README.md` & `eth-typing-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eth-typing-4.0.0/eth_typing/__init__.py` & `eth-typing-4.1.0/eth_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-typing-4.0.0/eth_typing/evm.py` & `eth-typing-4.1.0/eth_typing/evm.py`

 * *Files identical despite different names*

### Comparing `eth-typing-4.0.0/eth_typing/networks.py` & `eth-typing-4.1.0/eth_typing/networks.py`

 * *Files identical despite different names*

### Comparing `eth-typing-4.0.0/eth_typing.egg-info/PKG-INFO` & `eth-typing-4.1.0/eth_typing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 4.0.0
+Version: 4.1.0
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
```

### Comparing `eth-typing-4.0.0/pyproject.toml` & `eth-typing-4.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.autoflake]
-remove_all_unused_imports = true
 exclude = "__init__.py"
+remove_all_unused_imports = true
 
 [tool.isort]
 combine_as_imports = true
 extra_standard_library = "pytest"
 force_grid_wrap = 1
 force_sort_within_sections = true
-known_third_party = "hypothesis,pytest"
+honor_noqa = true
 known_first_party = "eth_typing"
+known_third_party = "hypothesis"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
 check_untyped_defs = true
-disallow_incomplete_defs = true
-disallow_untyped_defs = true
 disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
-disallow_subclassing_any = true
+disallow_untyped_defs = true
 ignore_missing_imports = true
-strict_optional = true
 strict_equality = true
+strict_optional = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 
 [tool.pydocstyle]
@@ -59,26 +61,26 @@
 # D400 - Enabling this error code seems to make it a requirement that the first
 # sentence in a docstring is not split across two lines.  It also makes it a
 # requirement that no docstring can have a multi-sentence description without a
 # summary line.  Neither one of those requirements seem appropriate.
 
 [tool.pytest.ini_options]
 addopts = "-v --showlocals --durations 10"
-xfail_strict = true
-log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 log_date_format = "%m-%d %H:%M:%S"
+log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
+xfail_strict = true
 
 [tool.towncrier]
 # Read https://github.com/ethereum/eth-typing/blob/main/newsfragments/README.md for instructions
-package = "eth_typing"
-filename = "docs/release_notes.rst"
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "eth-typing v{version} ({project_date})"
+filename = "docs/release_notes.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/eth-typing/issues/{issue}>`__"
+package = "eth_typing"
+title_format = "eth-typing v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `eth-typing-4.0.0/setup.py` & `eth-typing-4.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-typing",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="4.0.0",
+    version="4.1.0",
     description="""eth-typing: Common type annotations for ethereum python packages""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/eth-typing",
     include_package_data=True,
@@ -60,9 +60,10 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

