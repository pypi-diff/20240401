# Comparing `tmp/groundlight-0.9.0.tar.gz` & `tmp/groundlight-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.9.0.tar", max compression
+gzip compressed data, was "groundlight-0.9.1.tar", max compression
```

## Comparing `groundlight-0.9.0.tar` & `groundlight-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-06-15 23:03:07.003347 groundlight-0.9.0/LICENSE
--rw-r--r--   0        0        0     1868 2023-06-15 23:03:07.003347 groundlight-0.9.0/README.md
--rw-r--r--   0        0        0     3557 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/model.py
--rw-r--r--   0        0        0      752 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14047 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14351 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35605 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      539 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17676 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     5005 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11898 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13651 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13389 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11317 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13875 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11359 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12157 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12178 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11467 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79730 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1009 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14036 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/rest.py
--rw-r--r--   0        0        0     1013 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/setup.py
--rw-r--r--   0        0        0        0 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0     1804 2023-06-15 23:03:07.019347 groundlight-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      568 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/__init__.py
--rw-r--r--   0        0        0     2692 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0    11410 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/config.py
--rw-r--r--   0        0        0     2135 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/images.py
--rw-r--r--   0        0        0     6001 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1778 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0      308 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/status_codes.py
--rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 groundlight-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 19:10:07.613244 groundlight-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1868 2023-06-06 19:10:07.613444 groundlight-0.9.1/README.md
+-rw-r--r--   0        0        0     3557 2023-06-06 19:10:07.622673 groundlight-0.9.1/generated/model.py
+-rw-r--r--   0        0        0      752 2023-06-06 19:10:07.622761 groundlight-0.9.1/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-06 19:10:07.622856 groundlight-0.9.1/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14047 2023-06-06 19:10:07.622961 groundlight-0.9.1/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14351 2023-06-06 19:10:07.623043 groundlight-0.9.1/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35605 2023-06-06 19:10:07.623201 groundlight-0.9.1/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      539 2023-06-06 19:10:07.623302 groundlight-0.9.1/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17676 2023-06-06 19:10:07.623433 groundlight-0.9.1/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     5005 2023-06-06 19:10:07.623505 groundlight-0.9.1/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-06-06 19:10:07.623597 groundlight-0.9.1/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11898 2023-06-06 19:10:07.623712 groundlight-0.9.1/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13651 2023-06-06 19:10:07.623779 groundlight-0.9.1/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13389 2023-06-06 19:10:07.623871 groundlight-0.9.1/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11317 2023-06-06 19:10:07.623936 groundlight-0.9.1/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13875 2023-06-06 19:10:07.624004 groundlight-0.9.1/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11359 2023-06-06 19:10:07.624063 groundlight-0.9.1/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12157 2023-06-06 19:10:07.624123 groundlight-0.9.1/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12178 2023-06-06 19:10:07.624177 groundlight-0.9.1/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11467 2023-06-06 19:10:07.624227 groundlight-0.9.1/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79730 2023-06-06 19:10:07.624489 groundlight-0.9.1/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1009 2023-06-06 19:10:07.624588 groundlight-0.9.1/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14036 2023-06-06 19:10:07.624678 groundlight-0.9.1/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0     1013 2023-06-06 19:10:07.624842 groundlight-0.9.1/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-06-06 19:10:07.624955 groundlight-0.9.1/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-06-06 19:10:07.625024 groundlight-0.9.1/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-06-06 19:10:07.625077 groundlight-0.9.1/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-06-06 19:10:07.625125 groundlight-0.9.1/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-06-06 19:10:07.625173 groundlight-0.9.1/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-06-06 19:10:07.625236 groundlight-0.9.1/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-06-06 19:10:07.625299 groundlight-0.9.1/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-06-06 19:10:07.625346 groundlight-0.9.1/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-06-06 19:10:07.625395 groundlight-0.9.1/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-06-06 19:10:07.625443 groundlight-0.9.1/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-06-06 19:10:07.625496 groundlight-0.9.1/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-06-06 19:10:07.625596 groundlight-0.9.1/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0     1804 2023-06-30 18:59:31.610529 groundlight-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      568 2023-06-25 19:50:32.145320 groundlight-0.9.1/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     2692 2023-06-06 21:30:28.820411 groundlight-0.9.1/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0    11438 2023-06-30 18:59:09.410976 groundlight-0.9.1/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-06-06 19:10:07.628090 groundlight-0.9.1/src/groundlight/config.py
+-rw-r--r--   0        0        0     2909 2023-06-30 16:06:26.334960 groundlight-0.9.1/src/groundlight/images.py
+-rw-r--r--   0        0        0     8827 2023-06-30 16:06:26.335211 groundlight-0.9.1/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1778 2023-06-06 19:10:07.628295 groundlight-0.9.1/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0      432 2023-06-30 16:06:26.335374 groundlight-0.9.1/src/groundlight/status_codes.py
+-rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 groundlight-0.9.1/PKG-INFO
```

### Comparing `groundlight-0.9.0/LICENSE` & `groundlight-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/README.md` & `groundlight-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/model.py` & `groundlight-0.9.1/generated/model.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/__init__.py` & `groundlight-0.9.1/generated/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/api/detectors_api.py` & `groundlight-0.9.1/generated/openapi_client/api/detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.9.1/generated/openapi_client/api/image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/api_client.py` & `groundlight-0.9.1/generated/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/apis/__init__.py` & `groundlight-0.9.1/generated/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/configuration.py` & `groundlight-0.9.1/generated/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/exceptions.py` & `groundlight-0.9.1/generated/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/classification_result.py` & `groundlight-0.9.1/generated/openapi_client/model/classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/detector.py` & `groundlight-0.9.1/generated/openapi_client/model/detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.9.1/generated/openapi_client/model/detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.9.1/generated/openapi_client/model/detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/image_query.py` & `groundlight-0.9.1/generated/openapi_client/model/image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.9.1/generated/openapi_client/model/image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.9.1/generated/openapi_client/model/paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.9.1/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.9.1/generated/openapi_client/model/result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/model_utils.py` & `groundlight-0.9.1/generated/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/models/__init__.py` & `groundlight-0.9.1/generated/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/openapi_client/rest.py` & `groundlight-0.9.1/generated/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/setup.py` & `groundlight-0.9.1/generated/setup.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_classification_result.py` & `groundlight-0.9.1/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_detector.py` & `groundlight-0.9.1/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_detector_creation_input.py` & `groundlight-0.9.1/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_detector_type_enum.py` & `groundlight-0.9.1/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_detectors_api.py` & `groundlight-0.9.1/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_image_queries_api.py` & `groundlight-0.9.1/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_image_query.py` & `groundlight-0.9.1/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_image_query_type_enum.py` & `groundlight-0.9.1/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_paginated_detector_list.py` & `groundlight-0.9.1/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_paginated_image_query_list.py` & `groundlight-0.9.1/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/generated/test/test_result_type_enum.py` & `groundlight-0.9.1/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/pyproject.toml` & `groundlight-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = "MIT"
 name = "groundlight"
 packages = [
     {include = "**/*.py", from = "generated"},
     {include = "**/*.py", from = "src"},
 ]
 readme = "README.md"
-version = "0.9.0"
+version = "0.9.1"
 
 [tool.poetry.dependencies]
 certifi = "^2021.10.8"
 frozendict = "^2.3.2"
 pillow = "^9.0.0" # TODO: We may want to mark pillow (and numpy) as extra (https://python-poetry.org/docs/master/pyproject#extras)
 pydantic = "^1.7.4"
 python = ">=3.7.0,<4.0"
```

### Comparing `groundlight-0.9.0/src/groundlight/__init__.py` & `groundlight-0.9.1/src/groundlight/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/src/groundlight/binary_labels.py` & `groundlight-0.9.1/src/groundlight/binary_labels.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/src/groundlight/client.py` & `groundlight-0.9.1/src/groundlight/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 from openapi_client import Configuration
 from openapi_client.api.detectors_api import DetectorsApi
 from openapi_client.api.image_queries_api import ImageQueriesApi
 from openapi_client.model.detector_creation_input import DetectorCreationInput
 
 from groundlight.binary_labels import Label, convert_display_label_to_internal, convert_internal_label_to_display
 from groundlight.config import API_TOKEN_VARIABLE_NAME, API_TOKEN_WEB_URL
-from groundlight.images import parse_supported_image_types
-from groundlight.internalapi import GroundlightApiClient, NotFoundError, iq_is_confident, sanitize_endpoint_url
+from groundlight.images import ByteStreamWrapper, parse_supported_image_types
+from groundlight.internalapi import (
+    GroundlightApiClient,
+    NotFoundError,
+    iq_is_confident,
+    sanitize_endpoint_url,
+)
 from groundlight.optional_imports import Image, np
 
 logger = logging.getLogger("groundlight.sdk")
 
 
 class ApiTokenError(Exception):
     pass
@@ -177,15 +182,16 @@
           Any binary format must be JPEG-encoded already.  Any pixel format will get
           converted to JPEG at high quality before sending to service.
         :param wait: How long to wait (in seconds) for a confident answer.
         """
         if wait is None:
             wait = self.DEFAULT_WAIT
         detector_id = detector.id if isinstance(detector, Detector) else detector
-        image_bytesio: Union[BytesIO, BufferedReader] = parse_supported_image_types(image)
+
+        image_bytesio: ByteStreamWrapper = parse_supported_image_types(image)
 
         raw_image_query = self.image_queries_api.submit_image_query(detector_id=detector_id, body=image_bytesio)
         image_query = ImageQuery.parse_obj(raw_image_query.to_dict())
         if wait:
             threshold = self.get_detector(detector).confidence_threshold
             image_query = self.wait_for_confident_result(image_query, confidence_threshold=threshold, timeout_sec=wait)
         return self._fixup_image_query(image_query)
```

### Comparing `groundlight-0.9.0/src/groundlight/images.py` & `groundlight-0.9.1/src/groundlight/images.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 import imghdr
-from io import BufferedReader, BytesIO
+from io import BufferedReader, BytesIO, IOBase
 from typing import Union
 
 from groundlight.optional_imports import Image, np
 
 
+class ByteStreamWrapper(IOBase):
+    """This class acts as a thin wrapper around bytes in order to
+    maintain files in an open state. This is useful, in particular,
+    when we want to retry accessing the file without having to re-open it.
+    """
+
+    def __init__(self, data: Union[BufferedReader, BytesIO, bytes]) -> None:
+        super().__init__()
+        if isinstance(data, (BufferedReader, BytesIO)):
+            self._data = data.read()
+        else:
+            self._data = data
+
+    def read(self) -> bytes:
+        return self._data
+
+    def getvalue(self) -> bytes:
+        return self._data
+
+    def close(self) -> None:
+        pass
+
+
 def buffer_from_jpeg_file(image_filename: str) -> BufferedReader:
     """Get a buffer from an jpeg image file.
 
     For now, we only support JPEG files, and raise an ValueError otherwise.
     """
     if imghdr.what(image_filename) == "jpeg":
         # Note this will get fooled by truncated binaries since it only reads the header.
@@ -25,35 +48,36 @@
         out = buf.getvalue()
         return out
 
 
 def parse_supported_image_types(
     image: Union[str, bytes, Image.Image, BytesIO, BufferedReader, np.ndarray],
     jpeg_quality: int = 95,
-) -> Union[BytesIO, BufferedReader]:
+) -> ByteStreamWrapper:
     """Parse the many supported image types into a bytes-stream objects.
     In some cases we have to JPEG compress.
     """
     if isinstance(image, str):
         # Assume it is a filename
-        return buffer_from_jpeg_file(image)
+        buffer = buffer_from_jpeg_file(image)
+        return ByteStreamWrapper(data=buffer)
     if isinstance(image, bytes):
         # Create a BytesIO object
-        return BytesIO(image)
+        return ByteStreamWrapper(data=image)
     if isinstance(image, Image.Image):
         # Save PIL image as jpeg in BytesIO
         bytesio = BytesIO()
         image.save(bytesio, "jpeg", quality=jpeg_quality)
         bytesio.seek(0)
-        return bytesio
+        return ByteStreamWrapper(data=bytesio)
     if isinstance(image, (BytesIO, BufferedReader)):
         # Already in the right format
-        return image
+        return ByteStreamWrapper(data=image)
     if isinstance(image, np.ndarray):
         # Assume it is in BGR format from opencv
-        return BytesIO(jpeg_from_numpy(image[:, :, ::-1], jpeg_quality=jpeg_quality))
+        return ByteStreamWrapper(data=jpeg_from_numpy(image[:, :, ::-1], jpeg_quality=jpeg_quality))
     raise TypeError(
         (
-            "Unsupported type for image. Must be PIL, numpy (H,W,3) RGB, or a JPEG as a filename (str), bytes,"
+            "Unsupported type for image. Must be PIL, numpy (H,W,3) BGR, or a JPEG as a filename (str), bytes,"
             " BytesIO, or BufferedReader."
         ),
     )
```

### Comparing `groundlight-0.9.0/src/groundlight/internalapi.py` & `groundlight-0.9.1/src/groundlight/internalapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 import os
+import random
 import time
 import uuid
-from typing import Optional
+from functools import wraps
+from typing import Callable, Optional
 from urllib.parse import urlsplit, urlunsplit
 
 import requests
 from model import Detector, ImageQuery
-from openapi_client.api_client import ApiClient
+from openapi_client.api_client import ApiClient, ApiException
 
 from groundlight.status_codes import is_ok
 
 logger = logging.getLogger("groundlight.sdk")
 
 
 class NotFoundError(Exception):
@@ -63,27 +65,95 @@
     """
     if iq.result.confidence is None:
         # Human label
         return True
     return iq.result.confidence >= confidence_threshold
 
 
-class InternalApiError(RuntimeError):
-    # TODO: We need a better exception hierarchy
-    pass
+class InternalApiError(ApiException, RuntimeError):
+    # TODO: We should really avoid this double inheritance since
+    # both `ApiException` and `RuntimeError` are subclasses of
+    # `Exception`. Error handling might become more complex since
+    # the two super classes cross paths.
+    # pylint: disable=useless-super-delegation
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super().__init__(status, reason, http_resp)
+
+
+class RequestsRetryDecorator:
+    """
+    Decorate a function to retry sending HTTP requests.
+
+    Tries to re-execute the decorated function in case the execution
+    fails due to a server error (HTTP Error code 500 - 599).
+    Retry attempts are executed while exponentially backing off by a factor
+    of 2 with full jitter (picking a random delay time between 0 and the
+    maximum delay time).
+
+    """
+
+    def __init__(
+        self,
+        initial_delay: float = 0.2,
+        exponential_backoff: int = 2,
+        status_code_range: tuple = (500, 600),
+        max_retries: int = 3,
+    ):
+        self.initial_delay = initial_delay
+        self.exponential_backoff = exponential_backoff
+        self.status_code_range = range(*status_code_range)
+        self.max_retries = max_retries
+
+    def __call__(self, function: Callable) -> Callable:
+        """:param callable: The function to invoke."""
+
+        @wraps(function)
+        def decorated(*args, **kwargs):
+            delay = self.initial_delay
+            retry_count = 0
+
+            while retry_count <= self.max_retries:
+                try:
+                    return function(*args, **kwargs)
+                except ApiException as e:
+                    is_retryable = (e.status is not None) and (e.status in self.status_code_range)
+                    if not is_retryable:
+                        raise e
+                    if retry_count == self.max_retries:
+                        raise InternalApiError(reason="Maximum retries reached") from e
+
+                    if is_retryable:
+                        status_code = e.status
+                        if status_code in self.status_code_range:
+                            logger.warning(
+                                (
+                                    f"Current HTTP response status: {status_code}. "
+                                    f"Remaining retries: {self.max_retries - retry_count}"
+                                ),
+                                exc_info=True,
+                            )
+                            # This is implementing a full jitter strategy
+                            random_delay = random.uniform(0, delay)
+                            time.sleep(random_delay)
+
+                retry_count += 1
+                delay *= self.exponential_backoff
+
+        return decorated
 
 
 class GroundlightApiClient(ApiClient):
     """Subclassing the OpenAPI-generated ApiClient to add a bit of custom functionality.
     Not crazy about using polymorphism, but this is simpler than modifying the moustache
     templates in the generator to add the functionality.
     """
 
     REQUEST_ID_HEADER = "X-Request-Id"
 
+    @RequestsRetryDecorator()
     def call_api(self, *args, **kwargs):
         """Adds a request-id header to each API call."""
         # Note we don't look for header_param in kwargs here, because this method is only called in one place
         # in the generated code, so we can afford to make this brittle.
         header_param = args[4]  # that's the number in the list
         if not header_param:
             # This will never happen in normal usage.
@@ -93,23 +163,23 @@
             # Note that we have updated the actual dict in args, so we don't have to put it back in
         return super().call_api(*args, **kwargs)
 
     #
     # The methods below will eventually go away when we move to properly model
     # these methods with OpenAPI
     #
-
     def _headers(self) -> dict:
         request_id = _generate_request_id()
         return {
             "Content-Type": "application/json",
             "x-api-token": self.configuration.api_key["ApiToken"],
             "X-Request-Id": request_id,
         }
 
+    @RequestsRetryDecorator()
     def _add_label(self, image_query_id: str, label: str) -> dict:
         """Temporary internal call to add a label to an image query.  Not supported."""
         # TODO: Properly model this with OpenApi spec.
         start_time = time.time()
         url = f"{self.configuration.host}/labels"
 
         data = {
@@ -122,32 +192,33 @@
         logger.info(f"Posting label={label} to image_query {image_query_id} ...")
         response = requests.request("POST", url, json=data, headers=headers)
         elapsed = 1000 * (time.time() - start_time)
         logger.debug(f"Call to ImageQuery.add_label took {elapsed:.1f}ms response={response.text}")
 
         if not is_ok(response.status_code):
             raise InternalApiError(
-                f"Error adding label to image query {image_query_id} status={response.status_code} {response.text}",
+                status=response.status_code,
+                reason=f"Error adding label to image query {image_query_id}",
+                http_resp=response,
             )
 
         return response.json()
 
+    @RequestsRetryDecorator()
     def _get_detector_by_name(self, name: str) -> Detector:
         """Get a detector by name. For now, we use the list detectors API directly.
 
         TODO: Properly model this in the API, and generate SDK code for it.
         """
         url = f"{self.configuration.host}/v1/detectors?name={name}"
         headers = self._headers()
         response = requests.request("GET", url, headers=headers)
 
         if not is_ok(response.status_code):
-            raise InternalApiError(
-                f"Error getting detector by name '{name}' (status={response.status_code}): {response.text}",
-            )
+            raise InternalApiError(status=response.status_code, http_resp=response)
 
         parsed = response.json()
 
         if parsed["count"] == 0:
             raise NotFoundError(f"Detector with name={name} not found.")
         if parsed["count"] > 1:
             raise RuntimeError(
```

### Comparing `groundlight-0.9.0/src/groundlight/optional_imports.py` & `groundlight-0.9.1/src/groundlight/optional_imports.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.9.0/PKG-INFO` & `groundlight-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groundlight
-Version: 0.9.0
+Version: 0.9.1
 Summary: Build computer vision systems from natural language with Groundlight
 Home-page: https://code.groundlight.ai/python-sdk
 License: MIT
 Author: Groundlight AI
 Author-email: support@groundlight.ai
 Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

