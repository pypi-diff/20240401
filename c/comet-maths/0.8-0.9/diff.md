# Comparing `tmp/comet_maths-0.8.tar.gz` & `tmp/comet_maths-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\comet_maths-0.8.tar", last modified: Wed Jul 27 13:53:23 2022, max compression
+gzip compressed data, was "dist\comet_maths-0.9.tar", last modified: Wed Jul 27 14:01:34 2022, max compression
```

## Comparing `comet_maths-0.8.tar` & `comet_maths-0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/
--rw-rw-rw-   0        0        0     7797 2022-06-06 16:37:53.000000 comet_maths-0.8/LICENSE
--rw-rw-rw-   0        0        0       56 2022-05-03 15:16:11.000000 comet_maths-0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1796 2022-07-27 13:53:23.000000 comet_maths-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1235 2022-05-03 15:16:11.000000 comet_maths-0.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths/
--rw-rw-rw-   0        0        0     1065 2022-07-26 16:27:24.000000 comet_maths-0.8/comet_maths/__init__.py
--rw-rw-rw-   0        0        0    19024 2022-05-03 15:16:12.000000 comet_maths-0.8/comet_maths/_version.py
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths/interpolation/
--rw-rw-rw-   0        0        0        0 2021-11-18 10:16:42.000000 comet_maths-0.8/comet_maths/interpolation/__init__.py
--rw-rw-rw-   0        0        0    36950 2022-07-27 13:35:04.000000 comet_maths-0.8/comet_maths/interpolation/interpolation.py
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths/interpolation/tests/
--rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.8/comet_maths/interpolation/tests/__init__.py
--rw-rw-rw-   0        0        0    14409 2022-07-27 13:35:04.000000 comet_maths-0.8/comet_maths/interpolation/tests/test_interpolation.py
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths/linear_algebra/
--rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.8/comet_maths/linear_algebra/__init__.py
--rw-rw-rw-   0        0        0     8945 2022-07-27 13:35:03.000000 comet_maths-0.8/comet_maths/linear_algebra/matrix_calculation.py
--rw-rw-rw-   0        0        0    13356 2022-07-20 10:05:42.000000 comet_maths-0.8/comet_maths/linear_algebra/matrix_conversion.py
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths/linear_algebra/tests/
--rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.8/comet_maths/linear_algebra/tests/__init__.py
--rw-rw-rw-   0        0        0     1166 2022-07-26 16:48:58.000000 comet_maths-0.8/comet_maths/linear_algebra/tests/test_matrix_calculation.py
--rw-rw-rw-   0        0        0     4693 2022-07-20 10:05:42.000000 comet_maths-0.8/comet_maths/linear_algebra/tests/test_matrix_conversion.py
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths/random/
--rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.8/comet_maths/random/__init__.py
--rw-rw-rw-   0        0        0    11674 2022-07-27 13:35:04.000000 comet_maths-0.8/comet_maths/random/generate_sample.py
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths/random/tests/
--rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.8/comet_maths/random/tests/__init__.py
--rw-rw-rw-   0        0        0      503 2021-02-04 16:25:56.000000 comet_maths-0.8/comet_maths/random/tests/test_class_template.py
-drwxrwxrwx   0        0        0        0 2022-07-27 13:53:23.000000 comet_maths-0.8/comet_maths.egg-info/
--rw-rw-rw-   0        0        0     1796 2022-07-27 13:53:22.000000 comet_maths-0.8/comet_maths.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2022-07-27 13:53:22.000000 comet_maths-0.8/comet_maths.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-27 13:53:22.000000 comet_maths-0.8/comet_maths.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2022-07-27 13:53:22.000000 comet_maths-0.8/comet_maths.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-07-27 13:53:22.000000 comet_maths-0.8/comet_maths.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      475 2022-07-27 13:53:23.000000 comet_maths-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1221 2022-07-27 13:35:36.000000 comet_maths-0.8/setup.py
--rw-rw-rw-   0        0        0    70636 2022-05-03 15:16:11.000000 comet_maths-0.8/versioneer.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/
+-rw-rw-rw-   0        0        0     7797 2022-06-06 16:37:53.000000 comet_maths-0.9/LICENSE
+-rw-rw-rw-   0        0        0       56 2022-05-03 15:16:11.000000 comet_maths-0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1796 2022-07-27 14:01:34.000000 comet_maths-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1235 2022-05-03 15:16:11.000000 comet_maths-0.9/README.rst
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths/
+-rw-rw-rw-   0        0        0     1065 2022-07-26 16:27:24.000000 comet_maths-0.9/comet_maths/__init__.py
+-rw-rw-rw-   0        0        0    19024 2022-05-03 15:16:12.000000 comet_maths-0.9/comet_maths/_version.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths/interpolation/
+-rw-rw-rw-   0        0        0        0 2021-11-18 10:16:42.000000 comet_maths-0.9/comet_maths/interpolation/__init__.py
+-rw-rw-rw-   0        0        0    36954 2022-07-27 14:00:43.000000 comet_maths-0.9/comet_maths/interpolation/interpolation.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths/interpolation/tests/
+-rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.9/comet_maths/interpolation/tests/__init__.py
+-rw-rw-rw-   0        0        0    14409 2022-07-27 13:35:04.000000 comet_maths-0.9/comet_maths/interpolation/tests/test_interpolation.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths/linear_algebra/
+-rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.9/comet_maths/linear_algebra/__init__.py
+-rw-rw-rw-   0        0        0     8945 2022-07-27 13:35:03.000000 comet_maths-0.9/comet_maths/linear_algebra/matrix_calculation.py
+-rw-rw-rw-   0        0        0    13356 2022-07-20 10:05:42.000000 comet_maths-0.9/comet_maths/linear_algebra/matrix_conversion.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths/linear_algebra/tests/
+-rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.9/comet_maths/linear_algebra/tests/__init__.py
+-rw-rw-rw-   0        0        0     1166 2022-07-26 16:48:58.000000 comet_maths-0.9/comet_maths/linear_algebra/tests/test_matrix_calculation.py
+-rw-rw-rw-   0        0        0     4693 2022-07-20 10:05:42.000000 comet_maths-0.9/comet_maths/linear_algebra/tests/test_matrix_conversion.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths/random/
+-rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.9/comet_maths/random/__init__.py
+-rw-rw-rw-   0        0        0    11674 2022-07-27 13:35:04.000000 comet_maths-0.9/comet_maths/random/generate_sample.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths/random/tests/
+-rw-rw-rw-   0        0        0        0 2021-02-04 12:17:04.000000 comet_maths-0.9/comet_maths/random/tests/__init__.py
+-rw-rw-rw-   0        0        0      503 2021-02-04 16:25:56.000000 comet_maths-0.9/comet_maths/random/tests/test_class_template.py
+drwxrwxrwx   0        0        0        0 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths.egg-info/
+-rw-rw-rw-   0        0        0     1796 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-07-27 14:01:34.000000 comet_maths-0.9/comet_maths.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      475 2022-07-27 14:01:34.000000 comet_maths-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2022-07-27 14:01:05.000000 comet_maths-0.9/setup.py
+-rw-rw-rw-   0        0        0    70636 2022-05-03 15:16:11.000000 comet_maths-0.9/versioneer.py
```

### Comparing `comet_maths-0.8/LICENSE` & `comet_maths-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/PKG-INFO` & `comet_maths-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_maths
-Version: 0.8
+Version: 0.9
 Summary: Mathematical algorithms and tools to use within CoMet toolkit.
 Home-page: https://github.com/comet-toolkit/comet_maths
 Author: CoMet Toolkit Team
 Author-email: team@comet-toolkit.org
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
```

### Comparing `comet_maths-0.8/README.rst` & `comet_maths-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/__init__.py` & `comet_maths-0.9/comet_maths/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/_version.py` & `comet_maths-0.9/comet_maths/_version.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/interpolation/interpolation.py` & `comet_maths-0.9/comet_maths/interpolation/interpolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                 raise ValueError(
                     "comet_maths.interpolation: uncertainties for the model error for this interpolation method (%s) are not yet implemented"
                     % (method)
                 )
 
         if add_model_error or include_model_uncertainties:
             u_y_model, corr_y_model, cov_model = model_error_analytical_methods(
-                x_i, y_i, x, methods=unc_methods
+                x_i, y_i, x, unc_methods=unc_methods
             )
 
         if add_model_error:
             # y=cm.generate_sample(1,y,u_y_model,corr_y_model)
             y = cm.generate_sample_cov(1, y, cov_model, diff=0.1).squeeze()
 
         if (not return_uncertainties) and (not return_corr):
```

### Comparing `comet_maths-0.8/comet_maths/interpolation/tests/test_interpolation.py` & `comet_maths-0.9/comet_maths/interpolation/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/linear_algebra/matrix_calculation.py` & `comet_maths-0.9/comet_maths/linear_algebra/matrix_calculation.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/linear_algebra/matrix_conversion.py` & `comet_maths-0.9/comet_maths/linear_algebra/matrix_conversion.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/linear_algebra/tests/test_matrix_calculation.py` & `comet_maths-0.9/comet_maths/linear_algebra/tests/test_matrix_calculation.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/linear_algebra/tests/test_matrix_conversion.py` & `comet_maths-0.9/comet_maths/linear_algebra/tests/test_matrix_conversion.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths/random/generate_sample.py` & `comet_maths-0.9/comet_maths/random/generate_sample.py`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/comet_maths.egg-info/PKG-INFO` & `comet_maths-0.9/comet_maths.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet-maths
-Version: 0.8
+Version: 0.9
 Summary: Mathematical algorithms and tools to use within CoMet toolkit.
 Home-page: https://github.com/comet-toolkit/comet_maths
 Author: CoMet Toolkit Team
 Author-email: team@comet-toolkit.org
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
```

### Comparing `comet_maths-0.8/comet_maths.egg-info/SOURCES.txt` & `comet_maths-0.9/comet_maths.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comet_maths-0.8/setup.py` & `comet_maths-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     filename = os.path.join(os.path.dirname(__file__), filename)
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
-    version='0.8',
+    version='0.9',
     name="comet_maths",
     url="https://github.com/comet-toolkit/comet_maths",
     license="LGPLv3",
     author="CoMet Toolkit Team",
     author_email="team@comet-toolkit.org",
     description="Mathematical algorithms and tools to use within CoMet toolkit.",
     long_description=read("README.rst"),
```

### Comparing `comet_maths-0.8/versioneer.py` & `comet_maths-0.9/versioneer.py`

 * *Files identical despite different names*

