# Comparing `tmp/meringue-1.2.0.dev3.tar.gz` & `tmp/meringue-1.2.0.dev4.tar.gz`

## Comparing `meringue-1.2.0.dev3.tar` & `meringue-1.2.0.dev4.tar`

### file list

```diff
@@ -1,47 +1,51 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/apps.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/routers.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/docs/__init__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/docs/patchers.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/api/docs/views.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/conf/__init__.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/actions.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/apps.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/constants.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/drf_fields.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/exceptions.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/generators.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/images.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/properties.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/shortcuts.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/storage.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/templatetags/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/meringue/thumbnail/templatetags/m_thumbnails.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/LICENSE
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/README.md
--rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 meringue-1.2.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/apps.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/routers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/docs/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/docs/patchers.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/docs/views.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/conf/__init__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/apps.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/fields.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/views.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/actions.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/apps.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/constants.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/drf_fields.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/exceptions.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/generators.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/images.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/properties.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/shortcuts.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/storage.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/templatetags/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/templatetags/m_thumbnails.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/LICENSE
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/README.md
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/PKG-INFO
```

### Comparing `meringue-1.2.0.dev3/meringue/api/handlers.py` & `meringue-1.2.0.dev4/meringue/api/handlers.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 from django.http.response import Http404
 
 from rest_framework import exceptions
 from rest_framework import views
 
 from meringue.api.utils import render_error_details
 
+try:
+    from rest_framework_simplejwt.exceptions import DetailDictMixin
+except ImportError:
+    DetailDictMixin = None
+
 
 def exception_handler(exc, context):
     """
     Error handler returning message and error code pairs.
 
-    The handler is a wrapper over the standard handler [rest_framework.views.exception_handler][].
+    The handler is a wrapper over the standard handler `rest_framework.views.exception_handler`.
     """
 
     response = views.exception_handler(exc, context)
 
     if response is None:
         return response
 
     if isinstance(exc, (Http404, PermissionDenied)):
         # django Http404 and PermissionDenied errors are substituted for drf errors,
-        # in [rest_framework.views.exception_handler][] method.
+        # in `rest_framework.views.exception_handler` method.
         response.data = render_error_details(response.data["detail"])
 
+    elif DetailDictMixin and isinstance(exc, DetailDictMixin):
+        response.data = render_error_details(exc)
+
     elif isinstance(exc, exceptions.APIException):
         response.data = render_error_details(exc.detail)
 
     return response
```

### Comparing `meringue-1.2.0.dev3/meringue/api/routers.py` & `meringue-1.2.0.dev4/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/api/utils.py` & `meringue-1.2.0.dev4/meringue/api/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 from rest_framework.exceptions import ErrorDetail
 
+try:
+    from rest_framework_simplejwt.exceptions import DetailDictMixin
+except ImportError:
+    DetailDictMixin = None
+
 
 def render_error_details(error_detail: list | dict | ErrorDetail) -> list | dict:
     """
     The method renders errors of the ErrorDetail format into message and code pairs.
 
     Attributes:
         error_detail: Errors.
@@ -11,15 +16,21 @@
     Raises:
         Exception: Unknown error type.
 
     Returns:
         Rendered errors.
     """
 
-    if isinstance(error_detail, list):
+    if DetailDictMixin and isinstance(error_detail, DetailDictMixin):
+        return {
+            "message": error_detail.detail["detail"],
+            "code": error_detail.detail["code"],
+        }
+
+    elif isinstance(error_detail, list):
         error_list = [render_error_details(e) for e in error_detail]
         return error_list
 
     elif isinstance(error_detail, ErrorDetail):
         return {
             "message": str(error_detail),
             "code": error_detail.code,
```

### Comparing `meringue-1.2.0.dev3/meringue/api/docs/patchers.py` & `meringue-1.2.0.dev4/meringue/api/docs/patchers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/api/docs/views.py` & `meringue-1.2.0.dev4/meringue/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/conf/__init__.py` & `meringue-1.2.0.dev4/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/conf/default_settings.py` & `meringue-1.2.0.dev4/meringue/conf/default_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """
 Domain for generating absolute links
 """
 
 
 # API ##############################################################################################
 
-API_ENABLE_ROOT_VIEW: Final[str] = settings.DEBUG
+API_ENABLE_ROOT_VIEW: Final[bool] = settings.DEBUG
 """
 Option to enable or disable the root view of the [Router][meringue.api.routers.MeringueRouter]
 """
 
 
 # THUMBNAIL ########################################################################################
 
@@ -110,7 +110,18 @@
 
 THUMBNAIL_DUMMYIMAGE_TEMPLATE: Final[str] = "//dummyimage.com/{width}x{height}/9e9e9e/424242.png"
 
 THUMBNAIL_DEFAULT_FORMAT: Final[str] = "PNG"
 """
 Default thumbnail image format.
 """
+
+
+# PROTECTED ########################################################################################
+
+PROTECTED_SERVE_WITH_NGINX: Final[bool] = not settings.DEBUG
+"""
+The option implies the distribution of protected files by nginx. Instead of serving the file in
+response.
+
+The view [protected_file_view][meringue.protected.views.protected_file_view] adds the X-Accel-Redirect header with a link to the file.
+"""
```

### Comparing `meringue-1.2.0.dev3/meringue/core/models.py` & `meringue-1.2.0.dev4/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/query.py` & `meringue-1.2.0.dev4/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/translation.py` & `meringue-1.2.0.dev4/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/upload_handlers.py` & `meringue-1.2.0.dev4/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.2.0.dev4/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.2.0.dev4/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/templatetags/meringue_base.py` & `meringue-1.2.0.dev4/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/utils/crypt.py` & `meringue-1.2.0.dev4/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/utils/datetime.py` & `meringue-1.2.0.dev4/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/core/utils/frontend.py` & `meringue-1.2.0.dev4/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/actions.py` & `meringue-1.2.0.dev4/meringue/thumbnail/actions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/constants.py` & `meringue-1.2.0.dev4/meringue/thumbnail/constants.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/drf_fields.py` & `meringue-1.2.0.dev4/meringue/thumbnail/drf_fields.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/exceptions.py` & `meringue-1.2.0.dev4/meringue/thumbnail/exceptions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/generators.py` & `meringue-1.2.0.dev4/meringue/thumbnail/generators.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/images.py` & `meringue-1.2.0.dev4/meringue/thumbnail/images.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/properties.py` & `meringue-1.2.0.dev4/meringue/thumbnail/properties.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/shortcuts.py` & `meringue-1.2.0.dev4/meringue/thumbnail/shortcuts.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/storage.py` & `meringue-1.2.0.dev4/meringue/thumbnail/storage.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/meringue/thumbnail/templatetags/m_thumbnails.py` & `meringue-1.2.0.dev4/meringue/thumbnail/templatetags/m_thumbnails.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/LICENSE` & `meringue-1.2.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev3/README.md` & `meringue-1.2.0.dev4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	<a href="https://github.com/dd/Meringue/actions/workflows/mkdocs-release.yml" >
 		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/mkdocs-release.yml?logo=github&label=docs" alt="Documentation - Release" />
 	</a>
 	<a href="https://github.com/dd/Meringue/actions/workflows/test.yml" >
 		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/test.yml?logo=github&label=tests" alt="Tests - Running" />
 	</a>
 	<a href="https://codecov.io/gh/dd/Meringue" >
-		<img src="https://codecov.io/gh/dd/Meringue/branch/release/1.0.0/graph/badge.svg?token=HV1QGD74EK" alt="Tests - Coverage" />
+		<img src="https://codecov.io/gh/dd/Meringue/branch/master/graph/badge.svg?token=HV1QGD74EK" alt="Tests - Coverage" />
 	</a>
 </p>
 <p align="center">
 	<a href="https://github.com/pypa/hatch" target="_blank">
 		<img src="https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg" alt="Hatch project" />
 	</a>
 	<a href="https://squidfunk.github.io/mkdocs-material/" target="_blank">
@@ -54,15 +54,15 @@
 
 Package with various functional (such as mixins, form utils, upload handlers and other) for Django Framework.
 
 This library is a set of various functionality that I use from project to project.
 
 The main task of this package is to clean up this functionality, test it, and also organize the documentation so that colleagues can understand how and what works.
 
-However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
+However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@tovarisch.engineer), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 Read more in the [documentation](https://dd.github.io/Meringue/).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
@@ -72,15 +72,15 @@
 * [ ] Functionality for working with images.
 	* [x] Image editor like easy_thumbnails.
 	* [x] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
 	* [ ] Job chain presets
 	* [ ] Tests
 	* [ ] Docs
 * [ ] Functionality similar to that described in the previous paragraph only for video.
-* [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
+* [x] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -7,34 +7,34 @@
 and other) for Django Framework. This library is a set of various functionality
 that I use from project to project. The main task of this package is to clean
 up this functionality, test it, and also organize the documentation so that
 colleagues can understand how and what works. However, if someone decides to
 use this functionality in their project, and even more so to add functionality
 or change the implementation to a more correct, beautiful or understandable
 one, I will only be happy, do not worry and feel free to write to me by [mail]
-(mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/
-issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github]
-(https://github.com/dd/Meringue). Read more in the [documentation](https://
-dd.github.io/Meringue/). ## Roadmap Adding new functionality. Can change. * [ ]
-[drf](https://www.django-rest-framework.org/) serializer serializer for
-automatic form generation on the front when working through rest api. (An npm
-package on [vuejs](https://vuejs.org/) will also be developed generating form
-based on response from api). * [ ] Authorization backend for authorization by a
-pair of email and password. * [ ] Functionality for working with images. * [x]
-Image editor like easy_thumbnails. * [x] A field for the drf serializer that
-returns a set of images (for example, a standard image and a double-sized image
-for a retina screen), as well as in different formats (for example, in the
-original format and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs *
-[ ] Functionality similar to that described in the previous paragraph only for
-video. * [ ] Functionality for loading private files available through [nginx
-internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal). ##
-Contributing - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-
-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/
-gitflow-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https:/
-/github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
-github.com/psf/black) - [x] Lint commit with [Gitlint](https://
-jorisroovers.com/gitlint/) and [Conventional Commits](https://
-www.conventionalcommits.org/) - [x] Documentation with [mkdocs](https://
-www.mkdocs.org/) and [mkdocs-material](https://squidfunk.github.io/mkdocs-
-material/) - [x] Testing local with [hatch](https://hatch.pypa.io/1.7/meta/faq/
-#environments) - [x] Testing in CI/CD on push - [ ] Add [mypy](https://mypy-
-lang.org/) ???
+(mailto:dd@tovarisch.engineer), create an [issue](https://github.com/dd/
+Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on
+[github](https://github.com/dd/Meringue). Read more in the [documentation]
+(https://dd.github.io/Meringue/). ## Roadmap Adding new functionality. Can
+change. * [ ] [drf](https://www.django-rest-framework.org/) serializer
+serializer for automatic form generation on the front when working through rest
+api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
+generating form based on response from api). * [ ] Authorization backend for
+authorization by a pair of email and password. * [ ] Functionality for working
+with images. * [x] Image editor like easy_thumbnails. * [x] A field for the drf
+serializer that returns a set of images (for example, a standard image and a
+double-sized image for a retina screen), as well as in different formats (for
+example, in the original format and in webp). * [ ] Job chain presets * [ ]
+Tests * [ ] Docs * [ ] Functionality similar to that described in the previous
+paragraph only for video. * [x] Functionality for loading private files
+available through [nginx internal](http://nginx.org/en/docs/http/
+ngx_http_core_module.html#internal). ## Contributing - [x] Use Git Flow (read
+[here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://
+www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
+resolve the versioning - [x] Linter with a [Ruff](https://github.com/
+charliermarsh/ruff) - [x] Formatter with a [Black](https://github.com/psf/
+black) - [x] Lint commit with [Gitlint](https://jorisroovers.com/gitlint/) and
+[Conventional Commits](https://www.conventionalcommits.org/) - [x]
+Documentation with [mkdocs](https://www.mkdocs.org/) and [mkdocs-material]
+(https://squidfunk.github.io/mkdocs-material/) - [x] Testing local with [hatch]
+(https://hatch.pypa.io/1.7/meta/faq/#environments) - [x] Testing in CI/CD on
+push - [ ] Add [mypy](https://mypy-lang.org/) ???
```

### Comparing `meringue-1.2.0.dev3/pyproject.toml` & `meringue-1.2.0.dev4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "meringue"
 description = "A set of various functionality for a Django based web application."
 readme = "README.md"
 requires-python = ">=3.10"
 license = "LGPL-3.0"
 authors = [
-	{ name = "Dmitry Dobrynin", email = "dd@manin.space" },
+	{ name = "Dmitry Dobrynin", email = "dd@tovarisch.engineer" },
 ]
 keywords = ["django", "utils"]
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Environment :: Plugins",
 	"Environment :: Web Environment",
 	"Framework :: Django",
@@ -53,19 +53,18 @@
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 modeltranslation = ["django-modeltranslation>=0.17,<0.19"]
 drf = ["djangorestframework>=3.13,<4"]
 drf-spectacular = ["drf-spectacular>=0.26.3,<1"]
-cryptodome = ["pycryptodome==3.18.0"]
+cryptodome = ["pycryptodome==3.20.0"]
 
 [project.urls]
-"Homepage" = "https://github.com/dd/Meringue"
-"Documentation" = "https://dd.github.io/Meringue/"
+"Documentation" = "https://dd.github.io/Meringue"
 "Repository" = "https://github.com/dd/Meringue"
 "Changelog" = "https://github.com/dd/Meringue/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/dd/Meringue/issues"
 
 [tool.hatch.version]
 path = "meringue/__init__.py"
 
@@ -80,29 +79,29 @@
 	"CHANGELOG.md",
 	"CONTRIBUTING.md",
 	"tests",
 ]
 
 [tool.hatch.envs.default]
 description = "Dev environment"
-python = "3.11"
+python = "3.12"
 dependencies = [
-	"pre-commit==3.3.3",
-	"ipython==8.14.0",
-	"django==4.2",
-	"pytz==2023.3",
+	"pre-commit==3.5.0",
+	"ipython==8.17.1",
+	"django==4.2.7",
+	"pytz==2023.3.post1",
 	"django-modeltranslation==0.18.11",
-	"pycryptodome==3.18.0",
+	"pycryptodome==3.20.0",
 	"djangorestframework==3.14.0",
-	"drf-spectacular==0.26.4",
-	"Pillow==10.0.0",
+	"drf-spectacular==0.26.5",
+	"Pillow==10.1.0",
 ]
 [tool.hatch.envs.default.env-vars]
-DJANGO_SETTINGS_MODULE = 'test_project.settings'
-PYTHONPATH  = '.'
+DJANGO_SETTINGS_MODULE = "test_project.settings"
+PYTHONPATH  = "."
 [tool.hatch.envs.default.scripts]
 precommit_install = "pre-commit install {args}"
 precommit_uninstall = "pre-commit uninstall {args}"
 init = [
 	"git config --local gitflow.branch.master \"master\"",
 	"git config --local gitflow.branch.develop \"dev\"",
 	"git config --local gitflow.prefix.feature \"feature/\"",
@@ -111,28 +110,29 @@
 	"git config --local gitflow.prefix.hotfix \"hotfix/\"",
 	"git config --local gitflow.prefix.support \"support/\"",
 	"git config --local gitflow.prefix.versiontag \"v\"",
 	"git config --local gitflow.path.hooks $(pwd)\"/.git/hooks\"",
 	"precommit_install",
 ]
 remove = [
+	"git config --local --remove-section gitflow.branch",
+	"git config --local --remove-section gitflow.prefix",
+	"git config --local --remove-section gitflow.path",
 	"precommit_uninstall",
 ]
-makemessages = [
-	"cd meringue/core && django-admin makemessages -l en -l ru --no-obsolete {args}",
-]
+makemessages = "cd meringue/core && django-admin makemessages -l en -l ru --no-obsolete {args}"
 compilemessages = "cd meringue && django-admin compilemessages -l en -l ru {args}"
 
 [tool.hatch.envs.lint]
 description = "Lint environment"
 detached = true
 python = "3.11"
 dependencies = [
-	"ruff==0.0.280",
-	"black==23.7.0",
+	"ruff==0.3.4",
+	"black==24.3.0",
 ]
 [tool.hatch.envs.lint.scripts]
 check = [
 	"ruff {args:.}",
 	"black --check --diff --exclude=\".*migrations\\/.*$\" {args:.}",
 ]
 format = [
@@ -141,86 +141,98 @@
 ]
 
 [tool.hatch.envs.test]
 description = "Tests environment"
 detached = true
 python = "3.11"
 dependencies = [
-	"pytest==7.4.0",
+	"pytest==7.4.2",
 	"pytest-django==4.5.2",
 	"pytest-cov==4.1.0",
-	"Faker==19.2.0",
+	"Faker==19.6.1",
 	"django==4.2",
-	"pytz==2023.3",
+	"pytz==2023.3.post1",
 	"django-modeltranslation==0.18.11",
-	"pycryptodome==3.18.0",
+	"pycryptodome==3.20.0",
 	"djangorestframework==3.14.0",
+	"djangorestframework-simplejwt==5.3.1",
 	"drf-spectacular==0.26.4",
+	"pillow==10.3.0",
 ]
 [tool.hatch.envs.test.env-vars]
-DJANGO_SETTINGS_MODULE = 'test_project.settings'
-PYTHONPATH  = '.'
+DJANGO_SETTINGS_MODULE = "test_project.settings"
+PYTHONPATH  = "."
 [tool.hatch.envs.test.scripts]
 check = "pytest {args:--cov=meringue --cov-report term-missing}"
 makemigrations = "django-admin makemigrations {args}"
 
 [tool.hatch.envs.mtest]
 description = "Test matrix environment"
 detached = true
 dependencies = [
-	"pytest==7.4.0",
+	"pytest==7.4.2",
 	"pytest-django==4.5.2",
 	"pytest-cov==4.1.0",  # for ci tests with cover
-	"Faker==19.2.0",
-	"pytz==2023.3",
-	"pycryptodome==3.18.0",
+	"Faker==19.6.1",
+	"pytz==2023.3.post1",
+	"pycryptodome==3.20.0",
 	"drf-spectacular==0.26.4",
+	"pillow==10.3.0",
 ]
 [tool.hatch.envs.mtest.overrides]
 matrix.django.dependencies = [
 	{ value = "django~={matrix:django}" },
 	{ value = "django-modeltranslation=={matrix:modeltranslation}" },
 	{ value = "djangorestframework=={matrix:djangorestframework}" },
+	{ value = "djangorestframework-simplejwt=={matrix:simplejwt}" },
 ]
 [tool.hatch.envs.mtest.env-vars]
-DJANGO_SETTINGS_MODULE = 'test_project.settings'
-PYTHONPATH  = '.'
+DJANGO_SETTINGS_MODULE = "test_project.settings"
+PYTHONPATH  = "."
 [tool.hatch.envs.mtest.scripts]
 check = "pytest {args:-q}"
 [[tool.hatch.envs.mtest.matrix]]
 python = ["3.10", "3.11"]
 django = ["2.0"]
-modeltranslation = ["0.17.7"]
-djangorestframework = ["3.13.1"]
+modeltranslation = ["0.17.0"]
+djangorestframework = ["3.13.0"]
+simplejwt = ["5.2.0"]
+[[tool.hatch.envs.mtest.matrix]]
+python = ["3.10", "3.11"]
+django = ["3.0"]
+modeltranslation = ["0.17.0"]
+djangorestframework = ["3.13.0", "3.14.0", "3.15.0"]
+simplejwt = ["5.2.0", "5.3.0"]
 [[tool.hatch.envs.mtest.matrix]]
 python = ["3.10", "3.11"]
-django = ["3.0", "4.0"]
-modeltranslation = ["0.18.11"]
+django = ["4.0"]
+modeltranslation = ["0.17.0"]
 djangorestframework = ["3.14.0"]
+simplejwt = ["5.2.0", "5.3.0"]
 
 [tool.hatch.envs.docs]
 description = "Docs environment"
 detached = true
 python = "3.11"
 dependencies = [
-	"mkdocs[i18n]==1.5.1",
-	"mkdocs-literate-nav==0.6.0",
-	"mkdocs-material==9.1.21",
-	"mkdocs-git-revision-date-localized-plugin==1.2.0",
-	"mkdocs-git-authors-plugin==0.7.2",
-	"mkdocstrings[python]==0.22.0",
-	"black==23.7.0",
-	"mkdocs-minify-plugin==0.7.0",
+	"mkdocs[i18n]==1.5.3",
+	"mkdocs-literate-nav==0.6.1",
+	"mkdocs-material==9.5.16",
+	"mkdocs-git-revision-date-localized-plugin==1.2.4",
+	"mkdocs-git-authors-plugin==0.8.0",
+	"mkdocstrings[python]==0.24.1",
+	"black==24.3.0",
+	"mkdocs-minify-plugin==0.8.0",
 	"mkdocs-gen-files==0.5.0",
-	"Pygments==2.15.1",
+	"Pygments==2.17.2",
 	"mike==1.1.2",
-	"linkchecker==10.2.1",
+	"linkchecker==10.4.0",
 ]
 [tool.hatch.envs.docs.env-vars]
-MERINGUE_MKDOCS_ENABLE_MINIFY = 'false'
+MERINGUE_MKDOCS_ENABLE_MINIFY = "false"
 MKDOCS_CONFIG = "mkdocs.yml"
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --config-file {env:MKDOCS_CONFIG} --clean --strict {args}"
 serve = "mkdocs serve --config-file {env:MKDOCS_CONFIG} --dev-addr localhost:8000 {args}"
 ci-build = "mike deploy --config-file {env:MKDOCS_CONFIG} --update-aliases {args}"
 validate = "linkchecker --config .linkcheckerrc docs/dist"
 build-check = [
```

### Comparing `meringue-1.2.0.dev3/PKG-INFO` & `meringue-1.2.0.dev4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: meringue
-Version: 1.2.0.dev3
+Version: 1.2.0.dev4
 Summary: A set of various functionality for a Django based web application.
-Project-URL: Homepage, https://github.com/dd/Meringue
-Project-URL: Documentation, https://dd.github.io/Meringue/
+Project-URL: Documentation, https://dd.github.io/Meringue
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
-Author-email: Dmitry Dobrynin <dd@manin.space>
+Author-email: Dmitry Dobrynin <dd@tovarisch.engineer>
 License-Expression: LGPL-3.0
 License-File: AUTHORS
 License-File: LICENSE
 Keywords: django,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
@@ -44,15 +43,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: django>=1.11.17
 Provides-Extra: cryptodome
-Requires-Dist: pycryptodome==3.18.0; extra == 'cryptodome'
+Requires-Dist: pycryptodome==3.20.0; extra == 'cryptodome'
 Provides-Extra: drf
 Requires-Dist: djangorestframework<4,>=3.13; extra == 'drf'
 Provides-Extra: drf-spectacular
 Requires-Dist: drf-spectacular<1,>=0.26.3; extra == 'drf-spectacular'
 Provides-Extra: modeltranslation
 Requires-Dist: django-modeltranslation<0.19,>=0.17; extra == 'modeltranslation'
 Description-Content-Type: text/markdown
@@ -83,15 +82,15 @@
 	<a href="https://github.com/dd/Meringue/actions/workflows/mkdocs-release.yml" >
 		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/mkdocs-release.yml?logo=github&label=docs" alt="Documentation - Release" />
 	</a>
 	<a href="https://github.com/dd/Meringue/actions/workflows/test.yml" >
 		<img src="https://img.shields.io/github/actions/workflow/status/dd/Meringue/test.yml?logo=github&label=tests" alt="Tests - Running" />
 	</a>
 	<a href="https://codecov.io/gh/dd/Meringue" >
-		<img src="https://codecov.io/gh/dd/Meringue/branch/release/1.0.0/graph/badge.svg?token=HV1QGD74EK" alt="Tests - Coverage" />
+		<img src="https://codecov.io/gh/dd/Meringue/branch/master/graph/badge.svg?token=HV1QGD74EK" alt="Tests - Coverage" />
 	</a>
 </p>
 <p align="center">
 	<a href="https://github.com/pypa/hatch" target="_blank">
 		<img src="https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg" alt="Hatch project" />
 	</a>
 	<a href="https://squidfunk.github.io/mkdocs-material/" target="_blank">
@@ -113,15 +112,15 @@
 
 Package with various functional (such as mixins, form utils, upload handlers and other) for Django Framework.
 
 This library is a set of various functionality that I use from project to project.
 
 The main task of this package is to clean up this functionality, test it, and also organize the documentation so that colleagues can understand how and what works.
 
-However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
+However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@tovarisch.engineer), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 Read more in the [documentation](https://dd.github.io/Meringue/).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
@@ -131,15 +130,15 @@
 * [ ] Functionality for working with images.
 	* [x] Image editor like easy_thumbnails.
 	* [x] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
 	* [ ] Job chain presets
 	* [ ] Tests
 	* [ ] Docs
 * [ ] Functionality similar to that described in the previous paragraph only for video.
-* [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
+* [x] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.2.0.dev3 Summary: A set of
+Metadata-Version: 2.3 Name: meringue Version: 1.2.0.dev4 Summary: A set of
 various functionality for a Django based web application. Project-URL:
-Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
-dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
-Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
-Dmitry Dobrynin
-manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
-LICENSE Keywords: django,utils Classifier: Development Status :: 5 -
+Documentation, https://dd.github.io/Meringue Project-URL: Repository, https://
+github.com/dd/Meringue Project-URL: Changelog, https://github.com/dd/Meringue/
+blob/master/CHANGELOG.md Project-URL: Bug Tracker, https://github.com/dd/
+Meringue/issues Author-email: Dmitry Dobrynin
+tovarisch.engineer> License-Expression: LGPL-3.0 License-File: AUTHORS License-
+File: LICENSE Keywords: django,utils Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Plugins Classifier: Environment ::
 Web Environment Classifier: Framework :: Django Classifier: Framework :: Django
 :: 1 Classifier: Framework :: Django :: 1.11 Classifier: Framework :: Django ::
 2 Classifier: Framework :: Django :: 2.0 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4
@@ -23,15 +22,15 @@
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet ::
 WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=3.10 Requires-Dist: django>=1.11.17
-Provides-Extra: cryptodome Requires-Dist: pycryptodome==3.18.0; extra ==
+Provides-Extra: cryptodome Requires-Dist: pycryptodome==3.20.0; extra ==
 'cryptodome' Provides-Extra: drf Requires-Dist: djangorestframework<4,>=3.13;
 extra == 'drf' Provides-Extra: drf-spectacular Requires-Dist: drf-
 spectacular<1,>=0.26.3; extra == 'drf-spectacular' Provides-Extra:
 modeltranslation Requires-Dist: django-modeltranslation<0.19,>=0.17; extra ==
 'modeltranslation' Description-Content-Type: text/markdown
                             ************ MMeerriinngguuee ************
    _[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
@@ -42,34 +41,34 @@
 and other) for Django Framework. This library is a set of various functionality
 that I use from project to project. The main task of this package is to clean
 up this functionality, test it, and also organize the documentation so that
 colleagues can understand how and what works. However, if someone decides to
 use this functionality in their project, and even more so to add functionality
 or change the implementation to a more correct, beautiful or understandable
 one, I will only be happy, do not worry and feel free to write to me by [mail]
-(mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/
-issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github]
-(https://github.com/dd/Meringue). Read more in the [documentation](https://
-dd.github.io/Meringue/). ## Roadmap Adding new functionality. Can change. * [ ]
-[drf](https://www.django-rest-framework.org/) serializer serializer for
-automatic form generation on the front when working through rest api. (An npm
-package on [vuejs](https://vuejs.org/) will also be developed generating form
-based on response from api). * [ ] Authorization backend for authorization by a
-pair of email and password. * [ ] Functionality for working with images. * [x]
-Image editor like easy_thumbnails. * [x] A field for the drf serializer that
-returns a set of images (for example, a standard image and a double-sized image
-for a retina screen), as well as in different formats (for example, in the
-original format and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs *
-[ ] Functionality similar to that described in the previous paragraph only for
-video. * [ ] Functionality for loading private files available through [nginx
-internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal). ##
-Contributing - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-
-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/
-gitflow-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https:/
-/github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
-github.com/psf/black) - [x] Lint commit with [Gitlint](https://
-jorisroovers.com/gitlint/) and [Conventional Commits](https://
-www.conventionalcommits.org/) - [x] Documentation with [mkdocs](https://
-www.mkdocs.org/) and [mkdocs-material](https://squidfunk.github.io/mkdocs-
-material/) - [x] Testing local with [hatch](https://hatch.pypa.io/1.7/meta/faq/
-#environments) - [x] Testing in CI/CD on push - [ ] Add [mypy](https://mypy-
-lang.org/) ???
+(mailto:dd@tovarisch.engineer), create an [issue](https://github.com/dd/
+Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on
+[github](https://github.com/dd/Meringue). Read more in the [documentation]
+(https://dd.github.io/Meringue/). ## Roadmap Adding new functionality. Can
+change. * [ ] [drf](https://www.django-rest-framework.org/) serializer
+serializer for automatic form generation on the front when working through rest
+api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
+generating form based on response from api). * [ ] Authorization backend for
+authorization by a pair of email and password. * [ ] Functionality for working
+with images. * [x] Image editor like easy_thumbnails. * [x] A field for the drf
+serializer that returns a set of images (for example, a standard image and a
+double-sized image for a retina screen), as well as in different formats (for
+example, in the original format and in webp). * [ ] Job chain presets * [ ]
+Tests * [ ] Docs * [ ] Functionality similar to that described in the previous
+paragraph only for video. * [x] Functionality for loading private files
+available through [nginx internal](http://nginx.org/en/docs/http/
+ngx_http_core_module.html#internal). ## Contributing - [x] Use Git Flow (read
+[here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://
+www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
+resolve the versioning - [x] Linter with a [Ruff](https://github.com/
+charliermarsh/ruff) - [x] Formatter with a [Black](https://github.com/psf/
+black) - [x] Lint commit with [Gitlint](https://jorisroovers.com/gitlint/) and
+[Conventional Commits](https://www.conventionalcommits.org/) - [x]
+Documentation with [mkdocs](https://www.mkdocs.org/) and [mkdocs-material]
+(https://squidfunk.github.io/mkdocs-material/) - [x] Testing local with [hatch]
+(https://hatch.pypa.io/1.7/meta/faq/#environments) - [x] Testing in CI/CD on
+push - [ ] Add [mypy](https://mypy-lang.org/) ???
```

