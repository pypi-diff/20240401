# Comparing `tmp/cjunct-1.5.0.tar.gz` & `tmp/cjunct-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjunct-1.5.0.tar", max compression
+gzip compressed data, was "cjunct-1.6.0.tar", max compression
```

## Comparing `cjunct-1.5.0.tar` & `cjunct-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-1.5.0/LICENSE
--rw-r--r--   0        0        0     2428 2024-03-30 21:55:43.722425 cjunct-1.5.0/README.md
--rw-r--r--   0        0        0     4668 2024-03-30 18:13:01.471105 cjunct-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      525 2024-03-24 21:45:15.470380 cjunct-1.5.0/src/cjunct/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-1.5.0/src/cjunct/actions/__init__.py
--rw-r--r--   0        0        0     9930 2024-03-30 21:59:58.241247 cjunct-1.5.0/src/cjunct/actions/base.py
--rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-1.5.0/src/cjunct/actions/bundled/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-30 21:27:11.287640 cjunct-1.5.0/src/cjunct/actions/bundled/docker_shell.py
--rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-1.5.0/src/cjunct/actions/bundled/echo.py
--rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-1.5.0/src/cjunct/actions/bundled/shell.py
--rw-r--r--   0        0        0      283 2024-03-19 22:06:11.635010 cjunct-1.5.0/src/cjunct/actions/constants.py
--rw-r--r--   0        0        0     4524 2024-03-19 22:06:11.635657 cjunct-1.5.0/src/cjunct/actions/net.py
--rw-r--r--   0        0        0      177 2024-03-19 22:11:38.414830 cjunct-1.5.0/src/cjunct/actions/shell.py
--rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-1.5.0/src/cjunct/actions/types.py
--rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-1.5.0/src/cjunct/config/__init__.py
--rw-r--r--   0        0        0     3999 2024-03-30 21:50:09.818157 cjunct-1.5.0/src/cjunct/config/constants/__init__.py
--rw-r--r--   0        0        0     1170 2024-03-15 20:03:52.255938 cjunct-1.5.0/src/cjunct/config/constants/cli.py
--rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-1.5.0/src/cjunct/config/constants/helpers.py
--rw-r--r--   0        0        0     3339 2024-03-30 21:54:12.352156 cjunct-1.5.0/src/cjunct/config/environment.py
--rw-r--r--   0        0        0       79 2024-01-31 10:33:01.984083 cjunct-1.5.0/src/cjunct/config/loaders/__init__.py
--rw-r--r--   0        0        0    10681 2024-03-30 18:13:01.141669 cjunct-1.5.0/src/cjunct/config/loaders/base.py
--rw-r--r--   0        0        0        0 2024-01-31 10:33:01.985153 cjunct-1.5.0/src/cjunct/config/loaders/default/__init__.py
--rw-r--r--   0        0        0     2448 2024-03-30 22:01:24.282730 cjunct-1.5.0/src/cjunct/config/loaders/default/root.py
--rw-r--r--   0        0        0     5724 2024-03-30 21:59:58.226648 cjunct-1.5.0/src/cjunct/config/loaders/default/yaml.py
--rw-r--r--   0        0        0      963 2024-03-19 22:06:11.641292 cjunct-1.5.0/src/cjunct/config/loaders/helpers.py
--rw-r--r--   0        0        0     1931 2024-03-19 22:06:11.641758 cjunct-1.5.0/src/cjunct/config/loaders/inspect.py
--rw-r--r--   0        0        0     3534 2024-03-30 21:59:58.235230 cjunct-1.5.0/src/cjunct/console.py
--rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-1.5.0/src/cjunct/display/__init__.py
--rw-r--r--   0        0        0     1080 2024-03-20 09:52:53.055923 cjunct-1.5.0/src/cjunct/display/base.py
--rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-1.5.0/src/cjunct/display/color.py
--rw-r--r--   0        0        0     4389 2024-03-20 09:52:53.056699 cjunct-1.5.0/src/cjunct/display/default.py
--rw-r--r--   0        0        0     1335 2024-03-20 09:52:53.057410 cjunct-1.5.0/src/cjunct/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-1.5.0/src/cjunct/py.typed
--rw-r--r--   0        0        0     5110 2024-03-19 22:06:11.645780 cjunct-1.5.0/src/cjunct/rendering.py
--rw-r--r--   0        0        0     8638 2024-03-30 21:59:58.231437 cjunct-1.5.0/src/cjunct/runner.py
--rw-r--r--   0        0        0     6162 2024-03-23 08:21:43.685535 cjunct-1.5.0/src/cjunct/strategy.py
--rw-r--r--   0        0        0      393 2024-01-31 10:33:01.991091 cjunct-1.5.0/src/cjunct/types.py
--rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-1.5.0/src/cjunct/version.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:43:00.000000 cjunct-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2428 2024-03-31 11:43:25.516186 cjunct-1.6.0/README.md
+-rw-r--r--   0        0        0     4668 2024-04-01 12:40:21.559835 cjunct-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      525 2024-03-24 21:45:15.470380 cjunct-1.6.0/src/cjunct/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:06:11.631960 cjunct-1.6.0/src/cjunct/actions/__init__.py
+-rw-r--r--   0        0        0     9930 2024-03-31 11:43:25.517510 cjunct-1.6.0/src/cjunct/actions/base.py
+-rw-r--r--   0        0        0      233 2024-03-19 22:06:11.633239 cjunct-1.6.0/src/cjunct/actions/bundled/__init__.py
+-rw-r--r--   0        0        0     6568 2024-03-31 11:43:25.518075 cjunct-1.6.0/src/cjunct/actions/bundled/docker_shell.py
+-rw-r--r--   0        0        0      376 2024-03-19 22:06:11.633991 cjunct-1.6.0/src/cjunct/actions/bundled/echo.py
+-rw-r--r--   0        0        0     2138 2024-03-19 22:06:11.634519 cjunct-1.6.0/src/cjunct/actions/bundled/shell.py
+-rw-r--r--   0        0        0      283 2024-03-19 22:06:11.635010 cjunct-1.6.0/src/cjunct/actions/constants.py
+-rw-r--r--   0        0        0     4524 2024-03-19 22:06:11.635657 cjunct-1.6.0/src/cjunct/actions/net.py
+-rw-r--r--   0        0        0      177 2024-03-19 22:11:38.414830 cjunct-1.6.0/src/cjunct/actions/shell.py
+-rw-r--r--   0        0        0      456 2024-03-19 22:06:11.636689 cjunct-1.6.0/src/cjunct/actions/types.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:16:23.000000 cjunct-1.6.0/src/cjunct/config/__init__.py
+-rw-r--r--   0        0        0     4052 2024-04-01 12:40:21.560998 cjunct-1.6.0/src/cjunct/config/constants/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-01 11:54:38.652885 cjunct-1.6.0/src/cjunct/config/constants/cli.py
+-rw-r--r--   0        0        0     3412 2024-03-30 21:36:49.062570 cjunct-1.6.0/src/cjunct/config/constants/helpers.py
+-rw-r--r--   0        0        0     3339 2024-03-31 11:43:25.519612 cjunct-1.6.0/src/cjunct/config/environment.py
+-rw-r--r--   0        0        0       79 2024-01-31 10:33:01.984083 cjunct-1.6.0/src/cjunct/config/loaders/__init__.py
+-rw-r--r--   0        0        0    10681 2024-03-31 11:43:25.520459 cjunct-1.6.0/src/cjunct/config/loaders/base.py
+-rw-r--r--   0        0        0        0 2024-01-31 10:33:01.985153 cjunct-1.6.0/src/cjunct/config/loaders/default/__init__.py
+-rw-r--r--   0        0        0     2448 2024-03-31 11:43:25.521134 cjunct-1.6.0/src/cjunct/config/loaders/default/root.py
+-rw-r--r--   0        0        0     5724 2024-03-31 11:43:25.521583 cjunct-1.6.0/src/cjunct/config/loaders/default/yaml.py
+-rw-r--r--   0        0        0      963 2024-03-19 22:06:11.641292 cjunct-1.6.0/src/cjunct/config/loaders/helpers.py
+-rw-r--r--   0        0        0     1931 2024-03-19 22:06:11.641758 cjunct-1.6.0/src/cjunct/config/loaders/inspect.py
+-rw-r--r--   0        0        0     4983 2024-04-01 12:40:21.561983 cjunct-1.6.0/src/cjunct/console.py
+-rw-r--r--   0        0        0        0 2024-01-06 23:03:35.000000 cjunct-1.6.0/src/cjunct/display/__init__.py
+-rw-r--r--   0        0        0     1080 2024-03-20 09:52:53.055923 cjunct-1.6.0/src/cjunct/display/base.py
+-rw-r--r--   0        0        0      852 2024-03-19 22:06:11.643772 cjunct-1.6.0/src/cjunct/display/color.py
+-rw-r--r--   0        0        0     4389 2024-03-20 09:52:53.056699 cjunct-1.6.0/src/cjunct/display/default.py
+-rw-r--r--   0        0        0     1335 2024-03-20 09:52:53.057410 cjunct-1.6.0/src/cjunct/exceptions.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:43:00.000000 cjunct-1.6.0/src/cjunct/py.typed
+-rw-r--r--   0        0        0     5110 2024-03-19 22:06:11.645780 cjunct-1.6.0/src/cjunct/rendering.py
+-rw-r--r--   0        0        0     8638 2024-03-31 11:43:25.522927 cjunct-1.6.0/src/cjunct/runner.py
+-rw-r--r--   0        0        0     6162 2024-03-23 08:21:43.685535 cjunct-1.6.0/src/cjunct/strategy.py
+-rw-r--r--   0        0        0      393 2024-01-31 10:33:01.991091 cjunct-1.6.0/src/cjunct/types.py
+-rw-r--r--   0        0        0      348 2023-07-11 12:58:07.000000 cjunct-1.6.0/src/cjunct/version.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 cjunct-1.6.0/PKG-INFO
```

### Comparing `cjunct-1.5.0/LICENSE` & `cjunct-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/README.md` & `cjunct-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/pyproject.toml` & `cjunct-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cjunct"
-version = "1.5.0"
+version = "1.6.0"
 description = "Declarative task runner"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/cjunct"
```

### Comparing `cjunct-1.5.0/src/cjunct/__init__.py` & `cjunct-1.6.0/src/cjunct/__init__.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/actions/base.py` & `cjunct-1.6.0/src/cjunct/actions/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/actions/bundled/docker_shell.py` & `cjunct-1.6.0/src/cjunct/actions/bundled/docker_shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/actions/bundled/shell.py` & `cjunct-1.6.0/src/cjunct/actions/bundled/shell.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/actions/net.py` & `cjunct-1.6.0/src/cjunct/actions/net.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/constants/__init__.py` & `cjunct-1.6.0/src/cjunct/config/constants/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         lambda: Path().resolve(),
     )
     INTERACTIVE_MODE: Mandatory[bool] = Mandatory(
         lambda: get_cli_arg("interactive"),
         lambda: False,
     )
     ACTIONS_SOURCE_FILE: Optional[Path] = Optional(
+        lambda: maybe_path(get_cli_arg("workflow")),
         lambda: maybe_path(get_cli_arg("file")),
         lambda: maybe_path(Env.CJUNCT_WORKFLOW_FILE),
         lambda: maybe_path(Env.CJUNCT_ACTIONS_SOURCE_FILE),
     )
     CONFIG_LOADER_CLASS: Optional[LoaderClassType] = Optional(
         lambda: maybe_class_from_module(
             path_str=Env.CJUNCT_CONFIG_LOADER_SOURCE_FILE,
```

### Comparing `cjunct-1.5.0/src/cjunct/config/constants/cli.py` & `cjunct-1.6.0/src/cjunct/config/constants/cli.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/constants/helpers.py` & `cjunct-1.6.0/src/cjunct/config/constants/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/environment.py` & `cjunct-1.6.0/src/cjunct/config/environment.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/loaders/base.py` & `cjunct-1.6.0/src/cjunct/config/loaders/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/loaders/default/root.py` & `cjunct-1.6.0/src/cjunct/config/loaders/default/root.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/loaders/default/yaml.py` & `cjunct-1.6.0/src/cjunct/config/loaders/default/yaml.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/loaders/helpers.py` & `cjunct-1.6.0/src/cjunct/config/loaders/helpers.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/config/loaders/inspect.py` & `cjunct-1.6.0/src/cjunct/config/loaders/inspect.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/display/base.py` & `cjunct-1.6.0/src/cjunct/display/base.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/display/color.py` & `cjunct-1.6.0/src/cjunct/display/color.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/display/default.py` & `cjunct-1.6.0/src/cjunct/display/default.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/exceptions.py` & `cjunct-1.6.0/src/cjunct/exceptions.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/rendering.py` & `cjunct-1.6.0/src/cjunct/rendering.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/runner.py` & `cjunct-1.6.0/src/cjunct/runner.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/src/cjunct/strategy.py` & `cjunct-1.6.0/src/cjunct/strategy.py`

 * *Files identical despite different names*

### Comparing `cjunct-1.5.0/PKG-INFO` & `cjunct-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjunct
-Version: 1.5.0
+Version: 1.6.0
 Summary: Declarative task runner
 Home-page: https://github.com/reartnew/cjunct
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 4 - Beta
```

