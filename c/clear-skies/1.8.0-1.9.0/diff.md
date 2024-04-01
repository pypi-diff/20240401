# Comparing `tmp/clear-skies-1.8.0.tar.gz` & `tmp/clear-skies-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear-skies-1.8.0.tar", last modified: Mon Nov 21 11:24:05 2022, max compression
+gzip compressed data, was "clear-skies-1.9.0.tar", last modified: Tue Nov 22 15:04:28 2022, max compression
```

## Comparing `clear-skies-1.8.0.tar` & `clear-skies-1.9.0.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.246102 clear-skies-1.8.0/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2022-08-22 10:27:16.000000 clear-skies-1.8.0/LICENSE
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2022-08-22 10:27:16.000000 clear-skies-1.8.0/MANIFEST.in
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9007 2022-11-21 11:24:05.246102 clear-skies-1.8.0/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8322 2022-10-22 19:19:10.000000 clear-skies-1.8.0/README.md
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2022-11-21 11:24:05.246102 clear-skies-1.8.0/setup.cfg
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1452 2022-11-20 11:56:29.000000 clear-skies-1.8.0/setup.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.194100 clear-skies-1.8.0/src/
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.202101 clear-skies-1.8.0/src/clear_skies.egg-info/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9007 2022-11-21 11:24:05.000000 clear-skies-1.8.0/src/clear_skies.egg-info/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6684 2022-11-21 11:24:05.000000 clear-skies-1.8.0/src/clear_skies.egg-info/SOURCES.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2022-11-21 11:24:05.000000 clear-skies-1.8.0/src/clear_skies.egg-info/dependency_links.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       11 2022-11-21 11:24:05.000000 clear-skies-1.8.0/src/clear_skies.egg-info/requires.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       11 2022-11-21 11:24:05.000000 clear-skies-1.8.0/src/clear_skies.egg-info/top_level.txt
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.202101 clear-skies-1.8.0/src/clearskies/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      395 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      966 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/application.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.202101 clear-skies-1.8.0/src/clearskies/authentication/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      341 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/authentication/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4530 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/authentication/auth0_jwks.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       41 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/authentication/auth_exception.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      630 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/authentication/public.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1943 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/authentication/secret_bearer.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.202101 clear-skies-1.8.0/src/clearskies/autodoc/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       49 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.202101 clear-skies-1.8.0/src/clearskies/autodoc/formats/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       24 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.206101 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       85 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2992 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/oai3_json.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      507 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/oai3_schema_resolver.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1071 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/parameter.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2930 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/request.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      732 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/response.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.206101 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/schema/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      104 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/schema/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      310 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/schema/array.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      484 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/schema/default.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      265 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/schema/enum.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      853 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/schema/object.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.210101 clear-skies-1.8.0/src/clearskies/autodoc/request/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      158 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/request/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      236 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/request/header.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      240 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/request/json_body.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1322 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/request/request.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      249 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/request/url_parameter.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      239 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/request/url_path.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.210101 clear-skies-1.8.0/src/clearskies/autodoc/response/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       31 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/response/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      266 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/response/response.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.214101 clear-skies-1.8.0/src/clearskies/autodoc/schema/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      349 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      269 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/array.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      188 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/base64.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      246 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/boolean.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      186 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/date.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      195 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/datetime.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      190 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/double.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      392 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/enum.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      251 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/integer.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      190 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/long.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      249 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/number.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      383 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/object.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      194 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/password.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      244 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/autodoc/schema/string.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.218101 clear-skies-1.8.0/src/clearskies/backends/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      245 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/backends/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8728 2022-10-27 19:24:42.000000 clear-skies-1.8.0/src/clearskies/backends/api_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7430 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/backends/backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8726 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/backends/cursor_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    20881 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/backends/memory_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5521 2022-10-27 19:24:08.000000 clear-skies-1.8.0/src/clearskies/backends/restful_api_advanced_search_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2203 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/backends/secrets_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      455 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/binding_config.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.226101 clear-skies-1.8.0/src/clearskies/column_types/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1661 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10991 2022-11-02 14:18:01.000000 clear-skies-1.8.0/src/clearskies/column_types/belongs_to.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9822 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/column.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      304 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/created.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1783 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/datetime.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      345 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/email.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1246 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/float.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5944 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/has_many.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1326 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/integer.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      499 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/json.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11971 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/many_to_many.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7594 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/many_to_many_with_data.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      237 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/select.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      803 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/string.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      255 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/updated.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      676 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/column_types/uuid.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5538 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/columns.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6378 2022-10-26 17:11:30.000000 clear-skies-1.8.0/src/clearskies/condition_parser.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.226101 clear-skies-1.8.0/src/clearskies/contexts/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       67 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/bash.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1487 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/build_context.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1115 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/cli.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2483 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/context.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1429 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/convert_to_application.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1902 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/extract_handler.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2849 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/test.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      830 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/contexts/wsgi.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.230101 clear-skies-1.8.0/src/clearskies/di/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      123 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/di/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      526 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/di/additional_config.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    12825 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/di/di.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4102 2022-11-20 11:53:23.000000 clear-skies-1.8.0/src/clearskies/di/standard_dependencies.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.230101 clear-skies-1.8.0/src/clearskies/di/test_module/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       86 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/di/test_module/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.230101 clear-skies-1.8.0/src/clearskies/di/test_module/another_module/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       35 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/di/test_module/another_module/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       44 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/di/test_module/module_class.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3589 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/environment.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.230101 clear-skies-1.8.0/src/clearskies/functional/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       47 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/functional/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2808 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/functional/string.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      639 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/functional/validations.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.234102 clear-skies-1.8.0/src/clearskies/handlers/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      593 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    12564 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/advanced_search.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    21076 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/base.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11544 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/callable.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      922 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/create.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      433 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/crud_by_method.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1048 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/database_connector.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1832 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/delete.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.234102 clear-skies-1.8.0/src/clearskies/handlers/exceptions/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      190 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/exceptions/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       42 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/exceptions/authentication.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       41 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/exceptions/authorization.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       39 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/exceptions/client_error.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      136 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/exceptions/input_error.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       96 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/exceptions/not_found.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4450 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/get.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2032 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/health_check.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    22256 2022-11-08 18:09:18.000000 clear-skies-1.8.0/src/clearskies/handlers/list.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2751 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/mygrations.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1639 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/request_method_routing.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7563 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/restful_api.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3076 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/routing.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9272 2022-11-21 11:23:08.000000 clear-skies-1.8.0/src/clearskies/handlers/simple_routing.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6737 2022-11-21 11:23:08.000000 clear-skies-1.8.0/src/clearskies/handlers/simple_routing_route.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3896 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/simple_search.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1426 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/update.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10573 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/handlers/write.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.238102 clear-skies-1.8.0/src/clearskies/input_outputs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      107 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_outputs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5128 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_outputs/cli.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.238102 clear-skies-1.8.0/src/clearskies/input_outputs/exceptions/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       82 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_outputs/exceptions/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       41 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_outputs/exceptions/cli_input_error.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       39 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_outputs/exceptions/cli_not_found.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4386 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_outputs/input_output.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2967 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_outputs/wsgi.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.242102 clear-skies-1.8.0/src/clearskies/input_requirements/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      467 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_requirements/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      687 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_requirements/maximum_length.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      985 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_requirements/minimum_length.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1131 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_requirements/required.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_requirements/requirement.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      775 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/input_requirements/unique.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.242102 clear-skies-1.8.0/src/clearskies/mocks/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       65 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/mocks/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3288 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/mocks/input_output.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5120 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/mocks/models.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10728 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/model.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11989 2022-10-26 17:11:30.000000 clear-skies-1.8.0/src/clearskies/models.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.242102 clear-skies-1.8.0/src/clearskies/secrets/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      826 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/secrets/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.242102 clear-skies-1.8.0/src/clearskies/secrets/additional_configs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1114 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/secrets/additional_configs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2530 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5960 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7002 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/secrets/akeyless.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.246102 clear-skies-1.8.0/src/clearskies/security_headers/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      108 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/security_headers/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      243 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/security_headers/base.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3302 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/security_headers/cache_control.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3650 2022-11-08 16:34:45.000000 clear-skies-1.8.0/src/clearskies/security_headers/cors.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3885 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/security_headers/csp.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      761 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/security_headers/hsts.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/security_headers/x_content_type_options.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/security_headers/x_frame_options.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.246102 clear-skies-1.8.0/src/clearskies/tests/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/tests/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.246102 clear-skies-1.8.0/src/clearskies/tests/simple_api/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/tests/simple_api/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-21 11:24:05.246102 clear-skies-1.8.0/src/clearskies/tests/simple_api/models/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       50 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/tests/simple_api/models/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      643 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/tests/simple_api/models/status.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      771 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/tests/simple_api/models/user.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2095 2022-10-26 17:08:50.000000 clear-skies-1.8.0/src/clearskies/tests/simple_api/users_api.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.574323 clear-skies-1.9.0/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2022-08-22 10:27:16.000000 clear-skies-1.9.0/LICENSE
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2022-08-22 10:27:16.000000 clear-skies-1.9.0/MANIFEST.in
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9007 2022-11-22 15:04:28.574323 clear-skies-1.9.0/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8322 2022-10-22 19:19:10.000000 clear-skies-1.9.0/README.md
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2022-11-22 15:04:28.574323 clear-skies-1.9.0/setup.cfg
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1452 2022-11-22 15:03:55.000000 clear-skies-1.9.0/setup.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.518323 clear-skies-1.9.0/src/
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.522323 clear-skies-1.9.0/src/clear_skies.egg-info/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9007 2022-11-22 15:04:28.000000 clear-skies-1.9.0/src/clear_skies.egg-info/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6769 2022-11-22 15:04:28.000000 clear-skies-1.9.0/src/clear_skies.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2022-11-22 15:04:28.000000 clear-skies-1.9.0/src/clear_skies.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       11 2022-11-22 15:04:28.000000 clear-skies-1.9.0/src/clear_skies.egg-info/requires.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       11 2022-11-22 15:04:28.000000 clear-skies-1.9.0/src/clear_skies.egg-info/top_level.txt
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.526323 clear-skies-1.9.0/src/clearskies/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      395 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      966 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/application.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.526323 clear-skies-1.9.0/src/clearskies/authentication/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      382 2022-11-22 11:57:08.000000 clear-skies-1.9.0/src/clearskies/authentication/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4530 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/authentication/auth0_jwks.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       41 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/authentication/auth_exception.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      599 2022-11-22 11:58:26.000000 clear-skies-1.9.0/src/clearskies/authentication/authorization.py
+-rw-r--r--   0 cmancone  (1000) cmancone  (1000)     2680 2022-11-22 12:10:20.000000 clear-skies-1.9.0/src/clearskies/authentication/jwks.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      630 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/authentication/public.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1943 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/authentication/secret_bearer.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.526323 clear-skies-1.9.0/src/clearskies/autodoc/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       49 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.526323 clear-skies-1.9.0/src/clearskies/autodoc/formats/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       24 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.530323 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       85 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2992 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/oai3_json.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      507 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/oai3_schema_resolver.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1071 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/parameter.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2930 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/request.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      732 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/response.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.530323 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/schema/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      104 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/schema/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      310 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/schema/array.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      484 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/schema/default.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      265 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/schema/enum.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      853 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/schema/object.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.534323 clear-skies-1.9.0/src/clearskies/autodoc/request/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      158 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/request/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      236 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/request/header.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      240 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/request/json_body.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1322 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/request/request.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      249 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/request/url_parameter.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      239 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/request/url_path.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.534323 clear-skies-1.9.0/src/clearskies/autodoc/response/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       31 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/response/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      266 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/response/response.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.542323 clear-skies-1.9.0/src/clearskies/autodoc/schema/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      349 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      269 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/array.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      188 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/base64.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      246 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/boolean.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      186 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/date.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      195 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/datetime.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      190 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/double.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      392 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/enum.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      251 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/integer.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      190 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/long.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      249 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/number.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      383 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/object.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      194 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/password.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      244 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/autodoc/schema/string.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.542323 clear-skies-1.9.0/src/clearskies/backends/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      245 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/backends/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8728 2022-10-27 19:24:42.000000 clear-skies-1.9.0/src/clearskies/backends/api_backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7430 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/backends/backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8726 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/backends/cursor_backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    20881 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/backends/memory_backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5521 2022-10-27 19:24:08.000000 clear-skies-1.9.0/src/clearskies/backends/restful_api_advanced_search_backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2203 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/backends/secrets_backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      455 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/binding_config.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.550323 clear-skies-1.9.0/src/clearskies/column_types/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1661 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10991 2022-11-02 14:18:01.000000 clear-skies-1.9.0/src/clearskies/column_types/belongs_to.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9822 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/column.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      304 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/created.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1783 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/datetime.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      345 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/email.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1246 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/float.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5944 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/has_many.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1326 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/integer.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      499 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/json.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11971 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/many_to_many.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7594 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/many_to_many_with_data.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      237 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/select.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      803 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/string.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      255 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/updated.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      676 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/column_types/uuid.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5538 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/columns.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6378 2022-10-26 17:11:30.000000 clear-skies-1.9.0/src/clearskies/condition_parser.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.554323 clear-skies-1.9.0/src/clearskies/contexts/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       67 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/bash.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1487 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/build_context.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1115 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/cli.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2483 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/context.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1429 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/convert_to_application.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1902 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/extract_handler.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2994 2022-11-22 12:08:27.000000 clear-skies-1.9.0/src/clearskies/contexts/test.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      830 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/contexts/wsgi.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.554323 clear-skies-1.9.0/src/clearskies/di/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      123 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/di/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      526 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/di/additional_config.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    12825 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/di/di.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4102 2022-11-20 11:53:23.000000 clear-skies-1.9.0/src/clearskies/di/standard_dependencies.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.554323 clear-skies-1.9.0/src/clearskies/di/test_module/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       86 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/di/test_module/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.558323 clear-skies-1.9.0/src/clearskies/di/test_module/another_module/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       35 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/di/test_module/another_module/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       44 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/di/test_module/module_class.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3589 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/environment.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.558323 clear-skies-1.9.0/src/clearskies/functional/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       47 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/functional/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2808 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/functional/string.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      639 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/functional/validations.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.562323 clear-skies-1.9.0/src/clearskies/handlers/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      593 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    12564 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/advanced_search.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    22264 2022-11-22 14:05:35.000000 clear-skies-1.9.0/src/clearskies/handlers/base.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11544 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/callable.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      922 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/create.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      433 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/crud_by_method.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1048 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/database_connector.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1832 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/delete.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.562323 clear-skies-1.9.0/src/clearskies/handlers/exceptions/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      190 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/exceptions/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       42 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/exceptions/authentication.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       41 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/exceptions/authorization.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       39 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/exceptions/client_error.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      136 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/exceptions/input_error.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       96 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/exceptions/not_found.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4786 2022-11-22 14:07:34.000000 clear-skies-1.9.0/src/clearskies/handlers/get.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2032 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/health_check.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    22507 2022-11-22 00:41:16.000000 clear-skies-1.9.0/src/clearskies/handlers/list.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2751 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/mygrations.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1639 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/request_method_routing.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7563 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/restful_api.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3076 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/routing.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     9272 2022-11-21 11:23:08.000000 clear-skies-1.9.0/src/clearskies/handlers/simple_routing.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6737 2022-11-21 11:23:08.000000 clear-skies-1.9.0/src/clearskies/handlers/simple_routing_route.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3896 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/simple_search.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1426 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/update.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10573 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/handlers/write.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.562323 clear-skies-1.9.0/src/clearskies/input_outputs/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      107 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_outputs/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5128 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_outputs/cli.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.562323 clear-skies-1.9.0/src/clearskies/input_outputs/exceptions/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       82 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_outputs/exceptions/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       41 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_outputs/exceptions/cli_input_error.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       39 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_outputs/exceptions/cli_not_found.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     4386 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_outputs/input_output.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2967 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_outputs/wsgi.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.566323 clear-skies-1.9.0/src/clearskies/input_requirements/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      467 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_requirements/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      687 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_requirements/maximum_length.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      985 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_requirements/minimum_length.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1131 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_requirements/required.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_requirements/requirement.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      775 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/input_requirements/unique.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.566323 clear-skies-1.9.0/src/clearskies/mocks/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       65 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/mocks/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3376 2022-11-22 12:05:04.000000 clear-skies-1.9.0/src/clearskies/mocks/input_output.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5120 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/mocks/models.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10723 2022-11-21 23:53:40.000000 clear-skies-1.9.0/src/clearskies/model.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    11989 2022-10-26 17:11:30.000000 clear-skies-1.9.0/src/clearskies/models.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.566323 clear-skies-1.9.0/src/clearskies/secrets/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      826 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/secrets/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.570323 clear-skies-1.9.0/src/clearskies/secrets/additional_configs/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1114 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/secrets/additional_configs/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2530 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5960 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7002 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/secrets/akeyless.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.570323 clear-skies-1.9.0/src/clearskies/security_headers/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      108 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/security_headers/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      243 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/security_headers/base.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3302 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/security_headers/cache_control.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3650 2022-11-08 16:34:45.000000 clear-skies-1.9.0/src/clearskies/security_headers/cors.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3885 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/security_headers/csp.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      761 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/security_headers/hsts.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/security_headers/x_content_type_options.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/security_headers/x_frame_options.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.570323 clear-skies-1.9.0/src/clearskies/tests/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/tests/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.570323 clear-skies-1.9.0/src/clearskies/tests/simple_api/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/tests/simple_api/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2022-11-22 15:04:28.574323 clear-skies-1.9.0/src/clearskies/tests/simple_api/models/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       50 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/tests/simple_api/models/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      643 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/tests/simple_api/models/status.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      771 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/tests/simple_api/models/user.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2095 2022-10-26 17:08:50.000000 clear-skies-1.9.0/src/clearskies/tests/simple_api/users_api.py
```

### Comparing `clear-skies-1.8.0/LICENSE` & `clear-skies-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/PKG-INFO` & `clear-skies-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies
-Version: 1.8.0
+Version: 1.9.0
 Summary: A framework for building backends in the cloud
 Home-page: https://github.com/cmancone/clearskies
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `clear-skies-1.8.0/README.md` & `clear-skies-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/setup.py` & `clear-skies-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='clear-skies',
-    version='1.8.0',
+    version='1.9.0',
     description='A framework for building backends in the cloud',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cmancone/clearskies',
     author='Conor Mancone',
     author_email='cmancone@gmail.com',
     license='MIT',
```

### Comparing `clear-skies-1.8.0/src/clear_skies.egg-info/PKG-INFO` & `clear-skies-1.9.0/src/clear_skies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies
-Version: 1.8.0
+Version: 1.9.0
 Summary: A framework for building backends in the cloud
 Home-page: https://github.com/cmancone/clearskies
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `clear-skies-1.8.0/src/clear_skies.egg-info/SOURCES.txt` & `clear-skies-1.9.0/src/clear_skies.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 src/clearskies/condition_parser.py
 src/clearskies/environment.py
 src/clearskies/model.py
 src/clearskies/models.py
 src/clearskies/authentication/__init__.py
 src/clearskies/authentication/auth0_jwks.py
 src/clearskies/authentication/auth_exception.py
+src/clearskies/authentication/authorization.py
+src/clearskies/authentication/jwks.py
 src/clearskies/authentication/public.py
 src/clearskies/authentication/secret_bearer.py
 src/clearskies/autodoc/__init__.py
 src/clearskies/autodoc/formats/__init__.py
 src/clearskies/autodoc/formats/oai3_json/__init__.py
 src/clearskies/autodoc/formats/oai3_json/oai3_json.py
 src/clearskies/autodoc/formats/oai3_json/oai3_schema_resolver.py
```

### Comparing `clear-skies-1.8.0/src/clearskies/application.py` & `clear-skies-1.9.0/src/clearskies/application.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/authentication/auth0_jwks.py` & `clear-skies-1.9.0/src/clearskies/authentication/auth0_jwks.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/authentication/public.py` & `clear-skies-1.9.0/src/clearskies/authentication/public.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/authentication/secret_bearer.py` & `clear-skies-1.9.0/src/clearskies/authentication/secret_bearer.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/oai3_json.py` & `clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/oai3_json.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/parameter.py` & `clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/parameter.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/request.py` & `clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/request.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/response.py` & `clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/response.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/autodoc/formats/oai3_json/schema/object.py` & `clear-skies-1.9.0/src/clearskies/autodoc/formats/oai3_json/schema/object.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/autodoc/request/request.py` & `clear-skies-1.9.0/src/clearskies/autodoc/request/request.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/backends/api_backend.py` & `clear-skies-1.9.0/src/clearskies/backends/api_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/backends/backend.py` & `clear-skies-1.9.0/src/clearskies/backends/backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/backends/cursor_backend.py` & `clear-skies-1.9.0/src/clearskies/backends/cursor_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/backends/memory_backend.py` & `clear-skies-1.9.0/src/clearskies/backends/memory_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/backends/restful_api_advanced_search_backend.py` & `clear-skies-1.9.0/src/clearskies/backends/restful_api_advanced_search_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/backends/secrets_backend.py` & `clear-skies-1.9.0/src/clearskies/backends/secrets_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/__init__.py` & `clear-skies-1.9.0/src/clearskies/column_types/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/belongs_to.py` & `clear-skies-1.9.0/src/clearskies/column_types/belongs_to.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/column.py` & `clear-skies-1.9.0/src/clearskies/column_types/column.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/datetime.py` & `clear-skies-1.9.0/src/clearskies/column_types/datetime.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/float.py` & `clear-skies-1.9.0/src/clearskies/column_types/float.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/has_many.py` & `clear-skies-1.9.0/src/clearskies/column_types/has_many.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/integer.py` & `clear-skies-1.9.0/src/clearskies/column_types/integer.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/many_to_many.py` & `clear-skies-1.9.0/src/clearskies/column_types/many_to_many.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/many_to_many_with_data.py` & `clear-skies-1.9.0/src/clearskies/column_types/many_to_many_with_data.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/string.py` & `clear-skies-1.9.0/src/clearskies/column_types/string.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/column_types/uuid.py` & `clear-skies-1.9.0/src/clearskies/column_types/uuid.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/columns.py` & `clear-skies-1.9.0/src/clearskies/columns.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/condition_parser.py` & `clear-skies-1.9.0/src/clearskies/condition_parser.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/contexts/build_context.py` & `clear-skies-1.9.0/src/clearskies/contexts/build_context.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/contexts/cli.py` & `clear-skies-1.9.0/src/clearskies/contexts/cli.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/contexts/context.py` & `clear-skies-1.9.0/src/clearskies/contexts/context.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/contexts/convert_to_application.py` & `clear-skies-1.9.0/src/clearskies/contexts/convert_to_application.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/contexts/extract_handler.py` & `clear-skies-1.9.0/src/clearskies/contexts/extract_handler.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/contexts/test.py` & `clear-skies-1.9.0/src/clearskies/contexts/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         self,
         method=None,
         body=None,
         headers=None,
         url=None,
         routing_data=None,
         input_output=None,
-        query_parameters=None
+        query_parameters=None,
+        authorization_data=None,
     ):
         if self.application is None:
             raise ValueError("Cannot call the test context without an application")
 
         if input_output is None:
             input_output = InputOutput()
         if body is not None:
@@ -49,14 +50,16 @@
             input_output.set_request_method(method)
         if url is not None:
             input_output.set_request_url(url)
         if routing_data is not None:
             input_output.set_routing_data(routing_data)
         if query_parameters is not None:
             input_output.set_query_parameters(query_parameters)
+        if authorization_data is not None:
+            input_output.set_authorization_data(authorization_data)
 
         self.handler = self.di.build(self.application.handler_class, cache=False)
         self.handler.configure({
             **{
                 'authentication': public()
             },
             **self.application.handler_config,
```

### Comparing `clear-skies-1.8.0/src/clearskies/contexts/wsgi.py` & `clear-skies-1.9.0/src/clearskies/contexts/wsgi.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/di/additional_config.py` & `clear-skies-1.9.0/src/clearskies/di/additional_config.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/di/di.py` & `clear-skies-1.9.0/src/clearskies/di/di.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/di/standard_dependencies.py` & `clear-skies-1.9.0/src/clearskies/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/environment.py` & `clear-skies-1.9.0/src/clearskies/environment.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/functional/string.py` & `clear-skies-1.9.0/src/clearskies/functional/string.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/functional/validations.py` & `clear-skies-1.9.0/src/clearskies/functional/validations.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/__init__.py` & `clear-skies-1.9.0/src/clearskies/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/advanced_search.py` & `clear-skies-1.9.0/src/clearskies/handlers/advanced_search.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/base.py` & `clear-skies-1.9.0/src/clearskies/handlers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,25 @@
 
     def _check_configuration(self, configuration):
         if not 'authentication' in configuration:
             raise KeyError(
                 f"You must provide authentication in the configuration for handler '{self.__class__.__name__}'"
             )
         if configuration.get('authorization', None):
-            if not callable(configuration['authorization']) and not isinstance(configuration['authorization'], dict):
-                raise ValueError("'authorization' should be a callable or a dictionary with subclaims to enforce")
+            # authorization can be a function (in which case we'll just call it for gating) or it can be an object
+            # with 'gate' and 'filter_models' attributes, per the authentication.authorization base class
+            # or it can be a binding config
+            authorization = configuration['authorization']
+            if hasattr(authorization, 'object_class'):
+                # if it's a binding config then pull out the target class, since we just need to check attributes here
+                authorization = authorization.object_class
+            is_callable = callable(authorization)
+            gates_or_filters = hasattr(authorization, 'gate') or hasattr(authentication, 'filter_models')
+            if not is_callable and not gates_or_filters:
+                raise ValueError("'authorization' should be a callable or a provide 'gate' or 'filter_models' methods")
         if configuration.get('output_map') is not None:
             if not callable(configuration['output_map']):
                 raise ValueError("'output_map' should be a callable")
             signature = inspect.getfullargspec(configuration['output_map'])
             if signature.defaults and len(signature.defaults):
                 raise ValueError(
                     "'output_map' should be a callable that accepts one parameter: the model. " + \
@@ -108,14 +117,16 @@
         if key not in self._configuration:
             class_name = self.__class__.__name__
             raise KeyError(f"Configuration key '{key}' does not exist for handler '{class_name}'")
         return self._configuration[key]
 
     def _finalize_configuration(self, configuration):
         configuration['authentication'] = self._di.build(configuration['authentication'])
+        if configuration.get('authorization') and hasattr(configuration.get('authorization'), 'object_class'):
+            configuration['authorization'] = self._di.build(configuration['authorization'])
         if configuration.get('base_url') is None:
             configuration['base_url'] = '/'
         if not configuration['base_url'] or configuration['base_url'][0] != '/':
             configuration['base_url'] = '/' + configuration['base_url']
         security_headers = configuration.get('security_headers')
         if not security_headers:
             configuration['security_headers'] = []
@@ -150,16 +161,22 @@
         try:
             if not authentication.authenticate(input_output):
                 raise exceptions.Authentication('Not Authenticated')
         except exceptions.ClientError as client_error:
             raise exceptions.Authentication(str(client_error))
         authorization = self._configuration.get('authorization')
         if authorization:
+            authorization_data = input_output.get_authorization_data()
             try:
-                if not authentication.authorize(authorization):
+                allowed = True
+                if hasattr(authorization, 'gate'):
+                    allowed = authorization.gate(authorization_data, input_output)
+                elif callable(authorization):
+                    allowed = authorization(authorization_data, input_output)
+                if not allowed:
                     raise exceptions.Authorization('Not Authorized')
             except exceptions.ClientError as client_error:
                 raise exception.Authorization(str(client_error))
 
     def __call__(self, input_output):
         if self._configuration is None:
             raise ValueError("Must configure handler before calling")
```

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/callable.py` & `clear-skies-1.9.0/src/clearskies/handlers/callable.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/create.py` & `clear-skies-1.9.0/src/clearskies/handlers/create.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/database_connector.py` & `clear-skies-1.9.0/src/clearskies/handlers/database_connector.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/delete.py` & `clear-skies-1.9.0/src/clearskies/handlers/delete.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/get.py` & `clear-skies-1.9.0/src/clearskies/handlers/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,26 @@
         return self.success(input_output, self._model_as_json(model))
 
     def fetch_model(self, input_output):
         routing_data = input_output.routing_data()
         if 'id' not in routing_data:
             return "Missing 'id'"
         id = routing_data['id']
-        model = self._model.find(f'{self.id_column_name}={id}')
+        models = self._model.where(f'{self.id_column_name}={id}')
+        authorization = self._configuration.get('authorization', None)
+        if authorization and hasattr(authorization, 'filter_models'):
+            models = authorization.filter_models(models, input_output.get_authorization_data(), input_output)
+        model = models.first()
         if not model.exists:
             return "Not Found"
 
         return model
 
     def _check_configuration(self, configuration):
+        super()._check_configuration(configuration)
         error_prefix = 'Configuration error for %s:' % (self.__class__.__name__)
         has_model_class = ('model_class' in configuration) and configuration['model_class'] is not None
         has_model = ('model' in configuration) and configuration['model'] is not None
         if not has_model and not has_model_class:
             raise KeyError(f"{error_prefix} you must specify 'model' or 'model_class'")
         if has_model and has_model_class:
             raise KeyError(f"{error_prefix} you specified both 'model' and 'model_class', but can only provide one")
```

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/health_check.py` & `clear-skies-1.9.0/src/clearskies/handlers/health_check.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/list.py` & `clear-skies-1.9.0/src/clearskies/handlers/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
     def __init__(self, di):
         super().__init__(di)
 
     def handle(self, input_output):
         models = self._prepared_models.clone()
         limit = self.configuration('default_limit')
+        authorization = self._configuration.get('authorization', None)
+        if authorization and hasattr(authorization, 'filter_models'):
+            models = authorization.filter_models(models, input_output.get_authorization_data(), input_output)
         request_data = self.map_input_to_internal_names(input_output.request_data(False))
         query_parameters = self.map_input_to_internal_names(input_output.get_query_parameters())
         pagination_data = {}
         for key in self._model.allowed_pagination_keys():
             if key in request_data and key in query_parameters:
                 original_name = self.auto_case_internal_column_name(key)
                 return self.error(
```

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/mygrations.py` & `clear-skies-1.9.0/src/clearskies/handlers/mygrations.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/request_method_routing.py` & `clear-skies-1.9.0/src/clearskies/handlers/request_method_routing.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/restful_api.py` & `clear-skies-1.9.0/src/clearskies/handlers/restful_api.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/routing.py` & `clear-skies-1.9.0/src/clearskies/handlers/routing.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/simple_routing.py` & `clear-skies-1.9.0/src/clearskies/handlers/simple_routing.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/simple_routing_route.py` & `clear-skies-1.9.0/src/clearskies/handlers/simple_routing_route.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/simple_search.py` & `clear-skies-1.9.0/src/clearskies/handlers/simple_search.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/update.py` & `clear-skies-1.9.0/src/clearskies/handlers/update.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/handlers/write.py` & `clear-skies-1.9.0/src/clearskies/handlers/write.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/input_outputs/cli.py` & `clear-skies-1.9.0/src/clearskies/input_outputs/cli.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/input_outputs/input_output.py` & `clear-skies-1.9.0/src/clearskies/input_outputs/input_output.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/input_outputs/wsgi.py` & `clear-skies-1.9.0/src/clearskies/input_outputs/wsgi.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/input_requirements/maximum_length.py` & `clear-skies-1.9.0/src/clearskies/input_requirements/maximum_length.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/input_requirements/minimum_length.py` & `clear-skies-1.9.0/src/clearskies/input_requirements/minimum_length.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/input_requirements/required.py` & `clear-skies-1.9.0/src/clearskies/input_requirements/required.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/input_requirements/unique.py` & `clear-skies-1.9.0/src/clearskies/input_requirements/unique.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/mocks/input_output.py` & `clear-skies-1.9.0/src/clearskies/mocks/input_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,27 @@
         request_method='GET',
         request_url='',
         script_name='',
         path_info='',
         query_string='',
         content_type='',
         protocol='',
-        query_parameters=None
+        query_parameters=None,
+        authorization_data=None,
     ):
         self.set_request_method(request_method)
         self.set_body(body)
         self.set_request_headers(request_headers)
         self.set_request_url(request_url, script_name=script_name)
         self._path_info = path_info
         self._query_string = query_string
         self._content_type = content_type
         self._protocol = protocol
         self._query_parameters = query_parameters if query_parameters is not None else {}
+        self._authorization_data = authorization_data
 
     def respond(self, body, status_code=200):
         self.response = {'body': body, 'status_code': status_code, 'headers': self._response_headers}
         return (body, status_code)
 
     def get_body(self):
         return self._body
```

### Comparing `clear-skies-1.8.0/src/clearskies/mocks/models.py` & `clear-skies-1.9.0/src/clearskies/mocks/models.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/model.py` & `clear-skies-1.9.0/src/clearskies/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from collections import OrderedDict
 from .column_types import UUID
 from .functional import string
 import re
 from .models import Models
 class Model(Models):
     _configured_columns = None
```

### Comparing `clear-skies-1.8.0/src/clearskies/models.py` & `clear-skies-1.9.0/src/clearskies/models.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/secrets/__init__.py` & `clear-skies-1.9.0/src/clearskies/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/secrets/additional_configs/__init__.py` & `clear-skies-1.9.0/src/clearskies/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer.py` & `clear-skies-1.9.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear-skies-1.9.0/src/clearskies/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/secrets/akeyless.py` & `clear-skies-1.9.0/src/clearskies/secrets/akeyless.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/security_headers/cache_control.py` & `clear-skies-1.9.0/src/clearskies/security_headers/cache_control.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/security_headers/cors.py` & `clear-skies-1.9.0/src/clearskies/security_headers/cors.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/security_headers/csp.py` & `clear-skies-1.9.0/src/clearskies/security_headers/csp.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/security_headers/hsts.py` & `clear-skies-1.9.0/src/clearskies/security_headers/hsts.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/tests/simple_api/models/status.py` & `clear-skies-1.9.0/src/clearskies/tests/simple_api/models/status.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/tests/simple_api/models/user.py` & `clear-skies-1.9.0/src/clearskies/tests/simple_api/models/user.py`

 * *Files identical despite different names*

### Comparing `clear-skies-1.8.0/src/clearskies/tests/simple_api/users_api.py` & `clear-skies-1.9.0/src/clearskies/tests/simple_api/users_api.py`

 * *Files identical despite different names*

