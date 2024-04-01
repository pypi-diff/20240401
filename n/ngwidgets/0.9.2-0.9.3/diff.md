# Comparing `tmp/ngwidgets-0.9.2.tar.gz` & `tmp/ngwidgets-0.9.3.tar.gz`

## Comparing `ngwidgets-0.9.2.tar` & `ngwidgets-0.9.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/.components.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/.pydevproject
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/__init__.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/background.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/basetest.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/cmd.py
--rw-r--r--   0        0        0    13929 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/color_schema.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/components.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/components_view.py
--rw-r--r--   0        0        0    21391 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/dateparser.py
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/dict_edit.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/file_selector.py
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/input_webserver.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/leaflet.js
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/leaflet.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/local_filepicker.py
--rw-r--r--   0        0        0    14522 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/lod_grid.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/log_view.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/login.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/markup_header.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/ngwidgets_cmd.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/orjson_response.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/pdfviewer.js
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/pdfviewer.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/profiler.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/progress.py
--rw-r--r--   0        0        0    29032 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/projects.py
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/projects_view.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/tristate.js
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/tristate.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/users.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/version.py
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/webserver.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/webserver_test.py
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/widgets.py
--rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/widgets_demo.py
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets/yamlable.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets_examples/pdfviewer.html
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/ngwidgets_examples/show_example
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/scripts/install
--rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_color_schema.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_dateparser.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_file_selector.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_lod_grid.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_markup_header.py
--rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_nicegui_components.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_pdfviewer.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_webserver.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_widgets.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/tests/test_yamlable.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/LICENSE
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/README.md
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 ngwidgets-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/.components.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/.pydevproject
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/__init__.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/background.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/basetest.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/cmd.py
+-rw-r--r--   0        0        0    13929 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/color_schema.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/components.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/components_view.py
+-rw-r--r--   0        0        0    21391 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/dateparser.py
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/dict_edit.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/file_selector.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/input_webserver.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/leaflet.js
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/leaflet.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/local_filepicker.py
+-rw-r--r--   0        0        0    14522 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/lod_grid.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/log_view.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/login.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/markup_header.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/ngwidgets_cmd.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/orjson_response.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/pdfviewer.js
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/pdfviewer.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/profiler.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/progress.py
+-rw-r--r--   0        0        0    29032 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/projects.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/projects_view.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/tristate.js
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/tristate.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/users.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/version.py
+-rw-r--r--   0        0        0    10981 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/webserver.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/webserver_test.py
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/widgets.py
+-rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/widgets_demo.py
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets/yamlable.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets_examples/pdfviewer.html
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/ngwidgets_examples/show_example
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/scripts/install
+-rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_color_schema.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_dateparser.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_file_selector.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_lod_grid.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_markup_header.py
+-rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_nicegui_components.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_pdfviewer.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_webserver.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_widgets.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/tests/test_yamlable.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/README.md
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 ngwidgets-0.9.3/PKG-INFO
```

### Comparing `ngwidgets-0.9.2/.components.yaml` & `ngwidgets-0.9.3/.components.yaml`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/.github/workflows/build.yml` & `ngwidgets-0.9.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/.github/workflows/upload-to-pypi.yml` & `ngwidgets-0.9.3/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/background.py` & `ngwidgets-0.9.3/ngwidgets/background.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/basetest.py` & `ngwidgets-0.9.3/ngwidgets/basetest.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/cmd.py` & `ngwidgets-0.9.3/ngwidgets/cmd.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/color_schema.py` & `ngwidgets-0.9.3/ngwidgets/color_schema.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/components.py` & `ngwidgets-0.9.3/ngwidgets/components.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/components_view.py` & `ngwidgets-0.9.3/ngwidgets/components_view.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/dateparser.py` & `ngwidgets-0.9.3/ngwidgets/dateparser.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/dict_edit.py` & `ngwidgets-0.9.3/ngwidgets/dict_edit.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/file_selector.py` & `ngwidgets-0.9.3/ngwidgets/file_selector.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/input_webserver.py` & `ngwidgets-0.9.3/ngwidgets/input_webserver.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/leaflet.js` & `ngwidgets-0.9.3/ngwidgets/leaflet.js`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/leaflet.py` & `ngwidgets-0.9.3/ngwidgets/leaflet.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/local_filepicker.py` & `ngwidgets-0.9.3/ngwidgets/local_filepicker.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/lod_grid.py` & `ngwidgets-0.9.3/ngwidgets/lod_grid.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/log_view.py` & `ngwidgets-0.9.3/ngwidgets/log_view.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/login.py` & `ngwidgets-0.9.3/ngwidgets/login.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/markup_header.py` & `ngwidgets-0.9.3/ngwidgets/markup_header.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/ngwidgets_cmd.py` & `ngwidgets-0.9.3/ngwidgets/ngwidgets_cmd.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/pdfviewer.js` & `ngwidgets-0.9.3/ngwidgets/pdfviewer.js`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/pdfviewer.py` & `ngwidgets-0.9.3/ngwidgets/pdfviewer.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/profiler.py` & `ngwidgets-0.9.3/ngwidgets/profiler.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/progress.py` & `ngwidgets-0.9.3/ngwidgets/progress.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/projects.py` & `ngwidgets-0.9.3/ngwidgets/projects.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/projects_view.py` & `ngwidgets-0.9.3/ngwidgets/projects_view.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/tristate.py` & `ngwidgets-0.9.3/ngwidgets/tristate.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/users.py` & `ngwidgets-0.9.3/ngwidgets/users.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/version.py` & `ngwidgets-0.9.3/ngwidgets/version.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/webserver.py` & `ngwidgets-0.9.3/ngwidgets/webserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,20 @@
         """
         setup the footer
         """
         with ui.footer() as self.footer:
             ui.label(self.config.copy_right)
             ui.link("Powered by nicegui", "https://nicegui.io/").style("color: #fff")
 
+    def prepare_ui(self):
+        """
+        overridable function
+        """
+        pass
+    
     async def setup_content_div(
         self,
         setup_content: Optional[Callable] = None,
         with_exception_handling: bool = True,
         **kwargs,
     ):
         """
@@ -284,14 +290,15 @@
             setup_content (Optional[Callable]): A callable for setting up the main content.
                                                  It can be a regular function or a coroutine.
             with_exception_handling(bool): if True handle exceptions
 
         Note:
             This method is asynchronous and should be awaited when called.
         """
+        self.prepare_ui()
         # Setting up the menu
         self.setup_menu()
 
         with ui.element("div").classes("w-full h-full") as self.content_div:
             # Execute setup_content if provided
             if setup_content:
                 try:
```

### Comparing `ngwidgets-0.9.2/ngwidgets/webserver_test.py` & `ngwidgets-0.9.3/ngwidgets/webserver_test.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/widgets.py` & `ngwidgets-0.9.3/ngwidgets/widgets.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/widgets_demo.py` & `ngwidgets-0.9.3/ngwidgets/widgets_demo.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets/yamlable.py` & `ngwidgets-0.9.3/ngwidgets/yamlable.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/ngwidgets_examples/pdfviewer.html` & `ngwidgets-0.9.3/ngwidgets_examples/pdfviewer.html`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_color_schema.py` & `ngwidgets-0.9.3/tests/test_color_schema.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_dateparser.py` & `ngwidgets-0.9.3/tests/test_dateparser.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_file_selector.py` & `ngwidgets-0.9.3/tests/test_file_selector.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_lod_grid.py` & `ngwidgets-0.9.3/tests/test_lod_grid.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_markup_header.py` & `ngwidgets-0.9.3/tests/test_markup_header.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_nicegui_components.py` & `ngwidgets-0.9.3/tests/test_nicegui_components.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_pdfviewer.py` & `ngwidgets-0.9.3/tests/test_pdfviewer.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_webserver.py` & `ngwidgets-0.9.3/tests/test_webserver.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_widgets.py` & `ngwidgets-0.9.3/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/tests/test_yamlable.py` & `ngwidgets-0.9.3/tests/test_yamlable.py`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/.gitignore` & `ngwidgets-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/LICENSE` & `ngwidgets-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/README.md` & `ngwidgets-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/pyproject.toml` & `ngwidgets-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ngwidgets-0.9.2/PKG-INFO` & `ngwidgets-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngwidgets
-Version: 0.9.2
+Version: 0.9.3
 Summary: NiceGUI widgets and solution bazaar
 Project-URL: Home, https://github.com/WolfgangFahl/nicegui_widgets
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/nicegui_widgets
 Project-URL: Source, https://github.com/WolfgangFahl/nicegui_widgets
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
```

