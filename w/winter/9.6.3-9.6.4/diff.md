# Comparing `tmp/winter-9.6.3.tar.gz` & `tmp/winter-9.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winter-9.6.3.tar", max compression
+gzip compressed data, was "winter-9.6.4.tar", max compression
```

## Comparing `winter-9.6.3.tar` & `winter-9.6.4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0     1073 2022-07-15 06:57:00.585545 winter-9.6.3/LICENSE
--rw-r--r--   0        0        0     1819 2022-07-15 06:57:00.585545 winter-9.6.3/pyproject.toml
--rw-r--r--   0        0        0      823 2022-07-15 06:57:00.589545 winter-9.6.3/winter/__init__.py
--rw-r--r--   0        0        0      662 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/__init__.py
--rw-r--r--   0        0        0     1928 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/annotation_decorator.py
--rw-r--r--   0        0        0     2252 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/annotations.py
--rw-r--r--   0        0        0      654 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/application.py
--rw-r--r--   0        0        0     2147 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/component.py
--rw-r--r--   0        0        0     2903 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/component_method.py
--rw-r--r--   0        0        0     1380 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/component_method_argument.py
--rw-r--r--   0        0        0      564 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/docstring.py
--rw-r--r--   0        0        0      267 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/injection.py
--rw-r--r--   0        0        0      141 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/json/__init__.py
--rw-r--r--   0        0        0     9344 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/json/decoder.py
--rw-r--r--   0        0        0     3679 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/json/encoder.py
--rw-r--r--   0        0        0     1235 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/module_discovery.py
--rw-r--r--   0        0        0      215 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/utils/__init__.py
--rw-r--r--   0        0        0      164 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/utils/beautify_string.py
--rw-r--r--   0        0        0      546 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/utils/cached_property.py
--rw-r--r--   0        0        0      856 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/utils/nested_types.py
--rw-r--r--   0        0        0      540 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/utils/positive_integer.py
--rw-r--r--   0        0        0     1697 2022-07-15 06:57:00.589545 winter-9.6.3/winter/core/utils/typing.py
--rw-r--r--   0        0        0       39 2022-07-15 06:57:00.589545 winter-9.6.3/winter/data/__init__.py
--rw-r--r--   0        0        0      328 2022-07-15 06:57:00.589545 winter-9.6.3/winter/data/exceptions.py
--rw-r--r--   0        0        0      142 2022-07-15 06:57:00.589545 winter-9.6.3/winter/data/pagination/__init__.py
--rw-r--r--   0        0        0      394 2022-07-15 06:57:00.589545 winter-9.6.3/winter/data/pagination/page.py
--rw-r--r--   0        0        0      337 2022-07-15 06:57:00.589545 winter-9.6.3/winter/data/pagination/page_position.py
--rw-r--r--   0        0        0     1364 2022-07-15 06:57:00.589545 winter-9.6.3/winter/data/pagination/sort.py
--rw-r--r--   0        0        0     2014 2022-07-15 06:57:00.589545 winter-9.6.3/winter/data/repository.py
--rw-r--r--   0        0        0     3531 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/__init__.py
--rw-r--r--   0        0        0     3588 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/argument_resolver.py
--rw-r--r--   0        0        0      323 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/auth.py
--rw-r--r--   0        0        0      523 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/configurer.py
--rw-r--r--   0        0        0      266 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/controller.py
--rw-r--r--   0        0        0      694 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/default_response_status.py
--rw-r--r--   0        0        0      833 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exception_handlers.py
--rw-r--r--   0        0        0      416 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/__init__.py
--rw-r--r--   0        0        0      363 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/exception_handler_generator.py
--rw-r--r--   0        0        0      352 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/exception_mapper.py
--rw-r--r--   0        0        0      329 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/exceptions.py
--rw-r--r--   0        0        0     2592 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/handlers.py
--rw-r--r--   0        0        0      919 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/problem.py
--rw-r--r--   0        0        0      180 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/problem_annotation.py
--rw-r--r--   0        0        0     4318 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/problem_handling.py
--rw-r--r--   0        0        0      228 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/problem_handling_info.py
--rw-r--r--   0        0        0      970 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/exceptions/raises.py
--rw-r--r--   0        0        0      448 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/interceptor.py
--rw-r--r--   0        0        0     6056 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/media_type.py
--rw-r--r--   0        0        0     1928 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/output_processor.py
--rw-r--r--   0        0        0      132 2022-07-15 06:57:00.589545 winter-9.6.3/winter/web/pagination/__init__.py
--rw-r--r--   0        0        0      549 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/check_sort.py
--rw-r--r--   0        0        0     1192 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/limits.py
--rw-r--r--   0        0        0      620 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/order_by.py
--rw-r--r--   0        0        0      243 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/order_by_annotation.py
--rw-r--r--   0        0        0     3838 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/page_position_argument_resolver.py
--rw-r--r--   0        0        0     1020 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/page_processor.py
--rw-r--r--   0        0        0      486 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/page_processor_resolver.py
--rw-r--r--   0        0        0      504 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/parse_order.py
--rw-r--r--   0        0        0      336 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/parse_sort.py
--rw-r--r--   0        0        0     1169 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/pagination/utils.py
--rw-r--r--   0        0        0     1346 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/path_parameters_argument_resolver.py
--rw-r--r--   0        0        0      169 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/query_parameters/__init__.py
--rw-r--r--   0        0        0      269 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/query_parameters/map_query_parameter.py
--rw-r--r--   0        0        0      286 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/query_parameters/map_query_parameter_annotation.py
--rw-r--r--   0        0        0      114 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/query_parameters/query_parameter.py
--rw-r--r--   0        0        0     2662 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/query_parameters/query_parameters_argument_resolver.py
--rw-r--r--   0        0        0     1013 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/request_body_annotation.py
--rw-r--r--   0        0        0      819 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/request_body_resolver.py
--rw-r--r--   0        0        0      350 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/response_entity.py
--rw-r--r--   0        0        0     1703 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/response_header_annotation.py
--rw-r--r--   0        0        0     1250 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/response_header_resolver.py
--rw-r--r--   0        0        0     1536 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/response_header_serializer.py
--rw-r--r--   0        0        0     1028 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/response_header_serializers.py
--rw-r--r--   0        0        0      369 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/response_status_annotation.py
--rw-r--r--   0        0        0      319 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/routing/__init__.py
--rw-r--r--   0        0        0      247 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/routing/reverse.py
--rw-r--r--   0        0        0     1909 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/routing/route.py
--rw-r--r--   0        0        0      419 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/routing/route_annotation.py
--rw-r--r--   0        0        0     2437 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/routing/routing.py
--rw-r--r--   0        0        0     3045 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/throttling.py
--rw-r--r--   0        0        0     1780 2022-07-15 06:57:00.593545 winter-9.6.3/winter/web/urls.py
--rw-r--r--   0        0        0      243 2022-07-15 06:57:00.593545 winter-9.6.3/winter_ddd/__init__.py
--rw-r--r--   0        0        0      469 2022-07-15 06:57:00.593545 winter-9.6.3/winter_ddd/aggregate_root.py
--rw-r--r--   0        0        0       28 2022-07-15 06:57:00.593545 winter-9.6.3/winter_ddd/domain_event.py
--rw-r--r--   0        0        0     2020 2022-07-15 06:57:00.593545 winter-9.6.3/winter_ddd/domain_event_dispatcher.py
--rw-r--r--   0        0        0     1294 2022-07-15 06:57:00.593545 winter-9.6.3/winter_ddd/domain_event_handler.py
--rw-r--r--   0        0        0     1055 2022-07-15 06:57:00.593545 winter-9.6.3/winter_ddd/domain_event_subscription.py
--rw-r--r--   0        0        0      601 2022-07-15 06:57:00.593545 winter-9.6.3/winter_ddd/domain_events.py
--rw-r--r--   0        0        0      705 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/__init__.py
--rw-r--r--   0        0        0      355 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/autodiscovery.py
--rw-r--r--   0        0        0     1067 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/body_argument_resolver.py
--rw-r--r--   0        0        0      149 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/body_with_context.py
--rw-r--r--   0        0        0      629 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/http_request_argument_resolver.py
--rw-r--r--   0        0        0      742 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/input_serializer.py
--rw-r--r--   0        0        0      904 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/output_processor.py
--rw-r--r--   0        0        0     1027 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/output_serializer.py
--rw-r--r--   0        0        0      680 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/output_template.py
--rw-r--r--   0        0        0     1932 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/page_serializer.py
--rw-r--r--   0        0        0      157 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/renderers.py
--rw-r--r--   0        0        0     6062 2022-07-15 06:57:00.593545 winter-9.6.3/winter_django/view.py
--rw-r--r--   0        0        0     1563 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/__init__.py
--rw-r--r--   0        0        0      159 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/annotations/__init__.py
--rw-r--r--   0        0        0      707 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/annotations/global_exception.py
--rw-r--r--   0        0        0      219 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/enum_inspector.py
--rw-r--r--   0        0        0     3036 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/generation.py
--rw-r--r--   0        0        0      571 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/method_arguments_inspector.py
--rw-r--r--   0        0        0     1389 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/page_inspector.py
--rw-r--r--   0        0        0     2553 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/page_position_argument_inspector.py
--rw-r--r--   0        0        0     1713 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/path_parameters_inspector.py
--rw-r--r--   0        0        0     1899 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/query_parameters_inspector.py
--rw-r--r--   0        0        0     3438 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/swagger_auto_schema.py
--rw-r--r--   0        0        0     8232 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/type_inspection.py
--rw-r--r--   0        0        0     1510 2022-07-15 06:57:00.593545 winter-9.6.3/winter_openapi/validators.py
--rw-r--r--   0        0        0       86 2022-07-15 06:57:00.593545 winter-9.6.3/winter_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      730 2022-07-15 06:57:00.593545 winter-9.6.3/winter_sqlalchemy/query.py
--rw-r--r--   0        0        0     6546 2022-07-15 06:57:00.593545 winter-9.6.3/winter_sqlalchemy/repository.py
--rw-r--r--   0        0        0     1206 2022-07-15 06:57:39.519090 winter-9.6.3/setup.py
--rw-r--r--   0        0        0     1420 2022-07-15 06:57:39.519394 winter-9.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-08-01 13:22:52.630693 winter-9.6.4/LICENSE
+-rw-r--r--   0        0        0     1838 2022-08-01 13:22:52.630693 winter-9.6.4/pyproject.toml
+-rw-r--r--   0        0        0      823 2022-08-01 13:22:52.634693 winter-9.6.4/winter/__init__.py
+-rw-r--r--   0        0        0      662 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/__init__.py
+-rw-r--r--   0        0        0     1928 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/annotation_decorator.py
+-rw-r--r--   0        0        0     2252 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/annotations.py
+-rw-r--r--   0        0        0      654 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/application.py
+-rw-r--r--   0        0        0     2147 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/component.py
+-rw-r--r--   0        0        0     2903 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/component_method.py
+-rw-r--r--   0        0        0     1380 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/component_method_argument.py
+-rw-r--r--   0        0        0      564 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/docstring.py
+-rw-r--r--   0        0        0      267 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/injection.py
+-rw-r--r--   0        0        0      141 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/json/__init__.py
+-rw-r--r--   0        0        0     9344 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/json/decoder.py
+-rw-r--r--   0        0        0     3679 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/json/encoder.py
+-rw-r--r--   0        0        0     1235 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/module_discovery.py
+-rw-r--r--   0        0        0      215 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/utils/__init__.py
+-rw-r--r--   0        0        0      164 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/utils/beautify_string.py
+-rw-r--r--   0        0        0      546 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/utils/cached_property.py
+-rw-r--r--   0        0        0      856 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/utils/nested_types.py
+-rw-r--r--   0        0        0      540 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/utils/positive_integer.py
+-rw-r--r--   0        0        0     1697 2022-08-01 13:22:52.634693 winter-9.6.4/winter/core/utils/typing.py
+-rw-r--r--   0        0        0       39 2022-08-01 13:22:52.634693 winter-9.6.4/winter/data/__init__.py
+-rw-r--r--   0        0        0      328 2022-08-01 13:22:52.634693 winter-9.6.4/winter/data/exceptions.py
+-rw-r--r--   0        0        0      142 2022-08-01 13:22:52.634693 winter-9.6.4/winter/data/pagination/__init__.py
+-rw-r--r--   0        0        0      394 2022-08-01 13:22:52.634693 winter-9.6.4/winter/data/pagination/page.py
+-rw-r--r--   0        0        0      337 2022-08-01 13:22:52.634693 winter-9.6.4/winter/data/pagination/page_position.py
+-rw-r--r--   0        0        0     1364 2022-08-01 13:22:52.634693 winter-9.6.4/winter/data/pagination/sort.py
+-rw-r--r--   0        0        0     2014 2022-08-01 13:22:52.634693 winter-9.6.4/winter/data/repository.py
+-rw-r--r--   0        0        0     3531 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/__init__.py
+-rw-r--r--   0        0        0     3588 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/argument_resolver.py
+-rw-r--r--   0        0        0      323 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/auth.py
+-rw-r--r--   0        0        0      523 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/configurer.py
+-rw-r--r--   0        0        0      266 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/controller.py
+-rw-r--r--   0        0        0      694 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/default_response_status.py
+-rw-r--r--   0        0        0      833 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exception_handlers.py
+-rw-r--r--   0        0        0      416 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/__init__.py
+-rw-r--r--   0        0        0      363 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/exception_handler_generator.py
+-rw-r--r--   0        0        0      352 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/exception_mapper.py
+-rw-r--r--   0        0        0      329 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2592 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/handlers.py
+-rw-r--r--   0        0        0      919 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/problem.py
+-rw-r--r--   0        0        0      180 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/problem_annotation.py
+-rw-r--r--   0        0        0     4318 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/problem_handling.py
+-rw-r--r--   0        0        0      228 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/problem_handling_info.py
+-rw-r--r--   0        0        0      970 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/exceptions/raises.py
+-rw-r--r--   0        0        0      448 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/interceptor.py
+-rw-r--r--   0        0        0     6056 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/media_type.py
+-rw-r--r--   0        0        0     1928 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/output_processor.py
+-rw-r--r--   0        0        0      132 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/__init__.py
+-rw-r--r--   0        0        0      549 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/check_sort.py
+-rw-r--r--   0        0        0     1192 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/limits.py
+-rw-r--r--   0        0        0      620 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/order_by.py
+-rw-r--r--   0        0        0      243 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/order_by_annotation.py
+-rw-r--r--   0        0        0     3838 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/page_position_argument_resolver.py
+-rw-r--r--   0        0        0     1020 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/page_processor.py
+-rw-r--r--   0        0        0      486 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/page_processor_resolver.py
+-rw-r--r--   0        0        0      504 2022-08-01 13:22:52.634693 winter-9.6.4/winter/web/pagination/parse_order.py
+-rw-r--r--   0        0        0      336 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/pagination/parse_sort.py
+-rw-r--r--   0        0        0     1169 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/pagination/utils.py
+-rw-r--r--   0        0        0     1346 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/path_parameters_argument_resolver.py
+-rw-r--r--   0        0        0      169 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/query_parameters/__init__.py
+-rw-r--r--   0        0        0      269 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/query_parameters/map_query_parameter.py
+-rw-r--r--   0        0        0      286 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/query_parameters/map_query_parameter_annotation.py
+-rw-r--r--   0        0        0      114 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/query_parameters/query_parameter.py
+-rw-r--r--   0        0        0     2662 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/query_parameters/query_parameters_argument_resolver.py
+-rw-r--r--   0        0        0     1013 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/request_body_annotation.py
+-rw-r--r--   0        0        0      819 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/request_body_resolver.py
+-rw-r--r--   0        0        0      350 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/response_entity.py
+-rw-r--r--   0        0        0     1703 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/response_header_annotation.py
+-rw-r--r--   0        0        0     1250 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/response_header_resolver.py
+-rw-r--r--   0        0        0     1536 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/response_header_serializer.py
+-rw-r--r--   0        0        0     1028 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/response_header_serializers.py
+-rw-r--r--   0        0        0      369 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/response_status_annotation.py
+-rw-r--r--   0        0        0      319 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/routing/__init__.py
+-rw-r--r--   0        0        0      247 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/routing/reverse.py
+-rw-r--r--   0        0        0     1909 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/routing/route.py
+-rw-r--r--   0        0        0      419 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/routing/route_annotation.py
+-rw-r--r--   0        0        0     2437 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/routing/routing.py
+-rw-r--r--   0        0        0     3045 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/throttling.py
+-rw-r--r--   0        0        0     1780 2022-08-01 13:22:52.638693 winter-9.6.4/winter/web/urls.py
+-rw-r--r--   0        0        0      243 2022-08-01 13:22:52.638693 winter-9.6.4/winter_ddd/__init__.py
+-rw-r--r--   0        0        0      469 2022-08-01 13:22:52.638693 winter-9.6.4/winter_ddd/aggregate_root.py
+-rw-r--r--   0        0        0       28 2022-08-01 13:22:52.638693 winter-9.6.4/winter_ddd/domain_event.py
+-rw-r--r--   0        0        0     2020 2022-08-01 13:22:52.638693 winter-9.6.4/winter_ddd/domain_event_dispatcher.py
+-rw-r--r--   0        0        0     1294 2022-08-01 13:22:52.638693 winter-9.6.4/winter_ddd/domain_event_handler.py
+-rw-r--r--   0        0        0     1055 2022-08-01 13:22:52.638693 winter-9.6.4/winter_ddd/domain_event_subscription.py
+-rw-r--r--   0        0        0      601 2022-08-01 13:22:52.638693 winter-9.6.4/winter_ddd/domain_events.py
+-rw-r--r--   0        0        0      705 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/__init__.py
+-rw-r--r--   0        0        0      355 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/autodiscovery.py
+-rw-r--r--   0        0        0     1067 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/body_argument_resolver.py
+-rw-r--r--   0        0        0      149 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/body_with_context.py
+-rw-r--r--   0        0        0      629 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/http_request_argument_resolver.py
+-rw-r--r--   0        0        0      742 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/input_serializer.py
+-rw-r--r--   0        0        0      904 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/output_processor.py
+-rw-r--r--   0        0        0     1027 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/output_serializer.py
+-rw-r--r--   0        0        0      680 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/output_template.py
+-rw-r--r--   0        0        0     1932 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/page_serializer.py
+-rw-r--r--   0        0        0      157 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/renderers.py
+-rw-r--r--   0        0        0     6062 2022-08-01 13:22:52.638693 winter-9.6.4/winter_django/view.py
+-rw-r--r--   0        0        0     1563 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/__init__.py
+-rw-r--r--   0        0        0      159 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/annotations/__init__.py
+-rw-r--r--   0        0        0      707 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/annotations/global_exception.py
+-rw-r--r--   0        0        0      219 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/enum_inspector.py
+-rw-r--r--   0        0        0     3036 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/generation.py
+-rw-r--r--   0        0        0      571 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/method_arguments_inspector.py
+-rw-r--r--   0        0        0     1389 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/page_inspector.py
+-rw-r--r--   0        0        0     2553 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/page_position_argument_inspector.py
+-rw-r--r--   0        0        0     1713 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/path_parameters_inspector.py
+-rw-r--r--   0        0        0     1899 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/query_parameters_inspector.py
+-rw-r--r--   0        0        0     3438 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/swagger_auto_schema.py
+-rw-r--r--   0        0        0     8269 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/type_inspection.py
+-rw-r--r--   0        0        0     1510 2022-08-01 13:22:52.638693 winter-9.6.4/winter_openapi/validators.py
+-rw-r--r--   0        0        0       86 2022-08-01 13:22:52.638693 winter-9.6.4/winter_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      730 2022-08-01 13:22:52.638693 winter-9.6.4/winter_sqlalchemy/query.py
+-rw-r--r--   0        0        0     6546 2022-08-01 13:22:52.638693 winter-9.6.4/winter_sqlalchemy/repository.py
+-rw-r--r--   0        0        0     1232 2022-08-01 13:23:30.865755 winter-9.6.4/setup.py
+-rw-r--r--   0        0        0     1460 2022-08-01 13:23:30.866072 winter-9.6.4/PKG-INFO
```

### Comparing `winter-9.6.3/LICENSE` & `winter-9.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/pyproject.toml` & `winter-9.6.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "winter"
-version = "9.6.3"
+version = "9.6.4"
 homepage = "https://github.com/WinterFramework/winter"
 description = "Web Framework inspired by Spring Framework"
 authors = ["Alexander Egorov <mofr@zond.org>"]
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Development Status :: 3 - Alpha',
@@ -38,14 +38,15 @@
 docstring-parser = ">=0.1"
 drf-yasg = ">=1.13.0"
 furl = "2.0.0"
 python-dateutil = "2.8.0"
 injector = "0.15.0"
 SQLAlchemy = "~=1.3"
 typing-extensions = "^3.10.0"
+StrEnum = "^0.4.8"
 
 [tool.poetry.dev-dependencies]
 codecov = ">=2.0.9"
 flake8 = "3.7.7"
 flake8-commas = "2.0.0"
 flake8-formatter-abspath = "1.0.1"
 pre-commit-hooks = "2.2.3"
```

### Comparing `winter-9.6.3/winter/__init__.py` & `winter-9.6.4/winter/__init__.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/__init__.py` & `winter-9.6.4/winter/core/__init__.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/annotation_decorator.py` & `winter-9.6.4/winter/core/annotation_decorator.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/annotations.py` & `winter-9.6.4/winter/core/annotations.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/application.py` & `winter-9.6.4/winter/core/application.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/component.py` & `winter-9.6.4/winter/core/component.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/component_method.py` & `winter-9.6.4/winter/core/component_method.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/component_method_argument.py` & `winter-9.6.4/winter/core/component_method_argument.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/docstring.py` & `winter-9.6.4/winter/core/docstring.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/json/decoder.py` & `winter-9.6.4/winter/core/json/decoder.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/json/encoder.py` & `winter-9.6.4/winter/core/json/encoder.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/module_discovery.py` & `winter-9.6.4/winter/core/module_discovery.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/utils/cached_property.py` & `winter-9.6.4/winter/core/utils/cached_property.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/utils/nested_types.py` & `winter-9.6.4/winter/core/utils/nested_types.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/utils/positive_integer.py` & `winter-9.6.4/winter/core/utils/positive_integer.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/core/utils/typing.py` & `winter-9.6.4/winter/core/utils/typing.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/data/pagination/sort.py` & `winter-9.6.4/winter/data/pagination/sort.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/data/repository.py` & `winter-9.6.4/winter/data/repository.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/__init__.py` & `winter-9.6.4/winter/web/__init__.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/argument_resolver.py` & `winter-9.6.4/winter/web/argument_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/configurer.py` & `winter-9.6.4/winter/web/configurer.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/default_response_status.py` & `winter-9.6.4/winter/web/default_response_status.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/exception_handlers.py` & `winter-9.6.4/winter/web/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/exceptions/handlers.py` & `winter-9.6.4/winter/web/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/exceptions/problem.py` & `winter-9.6.4/winter/web/exceptions/problem.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/exceptions/problem_handling.py` & `winter-9.6.4/winter/web/exceptions/problem_handling.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/exceptions/raises.py` & `winter-9.6.4/winter/web/exceptions/raises.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/media_type.py` & `winter-9.6.4/winter/web/media_type.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/output_processor.py` & `winter-9.6.4/winter/web/output_processor.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/pagination/check_sort.py` & `winter-9.6.4/winter/web/pagination/check_sort.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/pagination/limits.py` & `winter-9.6.4/winter/web/pagination/limits.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/pagination/order_by.py` & `winter-9.6.4/winter/web/pagination/order_by.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/pagination/page_position_argument_resolver.py` & `winter-9.6.4/winter/web/pagination/page_position_argument_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/pagination/page_processor.py` & `winter-9.6.4/winter/web/pagination/page_processor.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/pagination/utils.py` & `winter-9.6.4/winter/web/pagination/utils.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/path_parameters_argument_resolver.py` & `winter-9.6.4/winter/web/path_parameters_argument_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/query_parameters/query_parameters_argument_resolver.py` & `winter-9.6.4/winter/web/query_parameters/query_parameters_argument_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/request_body_annotation.py` & `winter-9.6.4/winter/web/request_body_annotation.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/request_body_resolver.py` & `winter-9.6.4/winter/web/request_body_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/response_header_annotation.py` & `winter-9.6.4/winter/web/response_header_annotation.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/response_header_resolver.py` & `winter-9.6.4/winter/web/response_header_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/response_header_serializer.py` & `winter-9.6.4/winter/web/response_header_serializer.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/response_header_serializers.py` & `winter-9.6.4/winter/web/response_header_serializers.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/routing/route.py` & `winter-9.6.4/winter/web/routing/route.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/routing/routing.py` & `winter-9.6.4/winter/web/routing/routing.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/throttling.py` & `winter-9.6.4/winter/web/throttling.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter/web/urls.py` & `winter-9.6.4/winter/web/urls.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_ddd/domain_event_dispatcher.py` & `winter-9.6.4/winter_ddd/domain_event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_ddd/domain_event_handler.py` & `winter-9.6.4/winter_ddd/domain_event_handler.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_ddd/domain_event_subscription.py` & `winter-9.6.4/winter_ddd/domain_event_subscription.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_ddd/domain_events.py` & `winter-9.6.4/winter_ddd/domain_events.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/__init__.py` & `winter-9.6.4/winter_django/__init__.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/body_argument_resolver.py` & `winter-9.6.4/winter_django/body_argument_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/http_request_argument_resolver.py` & `winter-9.6.4/winter_django/http_request_argument_resolver.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/input_serializer.py` & `winter-9.6.4/winter_django/input_serializer.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/output_processor.py` & `winter-9.6.4/winter_django/output_processor.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/output_serializer.py` & `winter-9.6.4/winter_django/output_serializer.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/output_template.py` & `winter-9.6.4/winter_django/output_template.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/page_serializer.py` & `winter-9.6.4/winter_django/page_serializer.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_django/view.py` & `winter-9.6.4/winter_django/view.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/__init__.py` & `winter-9.6.4/winter_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/annotations/global_exception.py` & `winter-9.6.4/winter_openapi/annotations/global_exception.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/generation.py` & `winter-9.6.4/winter_openapi/generation.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/method_arguments_inspector.py` & `winter-9.6.4/winter_openapi/method_arguments_inspector.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/page_inspector.py` & `winter-9.6.4/winter_openapi/page_inspector.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/page_position_argument_inspector.py` & `winter-9.6.4/winter_openapi/page_position_argument_inspector.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/path_parameters_inspector.py` & `winter-9.6.4/winter_openapi/path_parameters_inspector.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/query_parameters_inspector.py` & `winter-9.6.4/winter_openapi/query_parameters_inspector.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/swagger_auto_schema.py` & `winter-9.6.4/winter_openapi/swagger_auto_schema.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_openapi/type_inspection.py` & `winter-9.6.4/winter_openapi/type_inspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 
 from drf_yasg import openapi
+from strenum import StrEnum
 
 from winter.core.utils import has_nested_type
 from winter.core.utils.typing import get_origin_type, get_generic_args
 from winter.core.utils.typing import is_any
 from winter.core.utils.typing import is_optional
 from winter.core.utils.typing import is_type_var
 
@@ -190,15 +191,15 @@
     if not args:
         return TypeInfo(openapi.TYPE_ARRAY, child=TypeInfo(TYPE_ANY_VALUE))
     child_class = args[0]
     child_type_info = inspect_type(child_class)
     return TypeInfo(openapi.TYPE_ARRAY, child=child_type_info)
 
 
-@register_type_inspector(enum.IntEnum, enum.Enum)
+@register_type_inspector(enum.IntEnum, StrEnum, enum.Enum)
 def inspect_enum(enum_class: Type[enum.Enum]) -> TypeInfo:
     enum_values = [entry.value for entry in enum_class]
     # Try to infer type based on enum values
     enum_value_types = {type(v) for v in enum_values}
 
     if len(enum_value_types) == 1:
         type_info = inspect_type(enum_value_types.pop())
```

### Comparing `winter-9.6.3/winter_openapi/validators.py` & `winter-9.6.4/winter_openapi/validators.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_sqlalchemy/query.py` & `winter-9.6.4/winter_sqlalchemy/query.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/winter_sqlalchemy/repository.py` & `winter-9.6.4/winter_sqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `winter-9.6.3/setup.py` & `winter-9.6.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Django<3.0.0',
  'SQLAlchemy>=1.3,<2.0',
+ 'StrEnum>=0.4.8,<0.5.0',
  'dataclasses>=0.6',
  'djangorestframework>=3.9.0',
  'docstring-parser>=0.1',
  'drf-yasg>=1.13.0',
  'furl==2.0.0',
  'injector==0.15.0',
  'python-dateutil==2.8.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'winter',
-    'version': '9.6.3',
+    'version': '9.6.4',
     'description': 'Web Framework inspired by Spring Framework',
     'long_description': None,
     'author': 'Alexander Egorov',
     'author_email': 'mofr@zond.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/WinterFramework/winter',
```

### Comparing `winter-9.6.3/PKG-INFO` & `winter-9.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winter
-Version: 9.6.3
+Version: 9.6.4
 Summary: Web Framework inspired by Spring Framework
 Home-page: https://github.com/WinterFramework/winter
 Author: Alexander Egorov
 Author-email: mofr@zond.org
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: Django (<3.0.0)
 Requires-Dist: SQLAlchemy (>=1.3,<2.0)
+Requires-Dist: StrEnum (>=0.4.8,<0.5.0)
 Requires-Dist: dataclasses (>=0.6)
 Requires-Dist: djangorestframework (>=3.9.0)
 Requires-Dist: docstring-parser (>=0.1)
 Requires-Dist: drf-yasg (>=1.13.0)
 Requires-Dist: furl (==2.0.0)
 Requires-Dist: injector (==0.15.0)
 Requires-Dist: python-dateutil (==2.8.0)
```

