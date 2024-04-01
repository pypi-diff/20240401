# Comparing `tmp/stigg_api_client_v2-1.98.0.tar.gz` & `tmp/stigg_api_client_v2-1.98.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-1.98.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-1.98.1.tar", max compression
```

## Comparing `stigg_api_client_v2-1.98.0.tar` & `stigg_api_client_v2-1.98.1.tar`

### file list

```diff
@@ -1,160 +1,160 @@
--rw-r--r--   0        0        0     5127 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/LICENSE
--rw-r--r--   0        0        0     1644 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/README.md
--rw-r--r--   0        0        0      549 2024-03-31 12:50:40.920106 stigg_api_client_v2-1.98.0/pyproject.toml
--rw-r--r--   0        0        0       62 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/__init__.py
--rw-r--r--   0        0        0    12780 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0    11617 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3521 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    24332 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     8481 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    30627 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     6266 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    26369 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0    13187 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0      611 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    98560 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    22227 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      783 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_git.py
--rw-r--r--   0        0        0      207 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0    16418 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0     5180 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_mock_val_ser.py
--rw-r--r--   0        0        0    28114 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4568 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4855 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0     6293 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_signature.py
--rw-r--r--   0        0        0    29094 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    17960 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12670 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3226 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0    10054 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0    11913 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_migration.py
--rw-r--r--   0        0        0     1600 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/alias_generators.py
--rw-r--r--   0        0        0     4162 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/aliases.py
--rw-r--r--   0        0        0     4357 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/annotated_handlers.py
--rw-r--r--   0        0        0      147 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/class_validators.py
--rw-r--r--   0        0        0    21493 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/color.py
--rw-r--r--   0        0        0    29141 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/config.py
--rw-r--r--   0        0        0    13450 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/dataclasses.py
--rw-r--r--   0        0        0      149 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/datetime_parse.py
--rw-r--r--   0        0        0      144 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/decorator.py
--rw-r--r--   0        0        0        0 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0     9871 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     2663 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7595 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10778 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4580 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2511 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     3336 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0      147 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/env_settings.py
--rw-r--r--   0        0        0      149 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4741 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/errors.py
--rw-r--r--   0        0        0    45930 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/fields.py
--rw-r--r--   0        0        0    14621 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    24317 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/functional_validators.py
--rw-r--r--   0        0        0      143 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/generics.py
--rw-r--r--   0        0        0      139 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/json.py
--rw-r--r--   0        0        0   102809 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/json_schema.py
--rw-r--r--   0        0        0    65892 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/main.py
--rw-r--r--   0        0        0    55135 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/mypy.py
--rw-r--r--   0        0        0    21225 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/networks.py
--rw-r--r--   0        0        0      140 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/parse.py
--rw-r--r--   0        0        0     6115 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/plugin/__init__.py
--rw-r--r--   0        0        0     1858 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/plugin/_loader.py
--rw-r--r--   0        0        0     5228 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/plugin/_schema_validator.py
--rw-r--r--   0        0        0        0 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/py.typed
--rw-r--r--   0        0        0     5599 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/root_model.py
--rw-r--r--   0        0        0      141 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/schema.py
--rw-r--r--   0        0        0      140 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/tools.py
--rw-r--r--   0        0        0    18108 2024-03-31 12:49:33.720866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/type_adapter.py
--rw-r--r--   0        0        0    89609 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/types.py
--rw-r--r--   0        0        0      137 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/typing.py
--rw-r--r--   0        0        0      140 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/utils.py
--rw-r--r--   0        0        0     2771 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    15026 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/color.py
--rw-r--r--   0        0        0     6477 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/config.py
--rw-r--r--   0        0        0    18073 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    14039 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5141 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50485 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17805 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/json.py
--rw-r--r--   0        0        0    44376 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/main.py
--rw-r--r--   0        0        0    38748 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    22059 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47614 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2826 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35379 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/types.py
--rw-r--r--   0        0        0    18996 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/utils.py
--rw-r--r--   0        0        0    21887 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1039 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/version.py
--rw-r--r--   0        0        0     2054 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/validate_call_decorator.py
--rw-r--r--   0        0        0      145 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/validators.py
--rw-r--r--   0        0        0     2560 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/version.py
--rw-r--r--   0        0        0     2322 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/warnings.py
--rw-r--r--   0        0        0        4 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/INSTALLER
--rw-r--r--   0        0        0    85087 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/METADATA
--rw-r--r--   0        0        0    14262 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/RECORD
--rw-r--r--   0        0        0        0 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/WHEEL
--rw-r--r--   0        0        0     1129 2024-03-31 12:49:33.716866 stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     6886 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/client.py
--rw-r--r--   0        0        0     1455 2024-03-31 12:49:33.724866 stigg_api_client_v2-1.98.0/stigg/edge_utils.py
--rw-r--r--   0        0        0    57568 2024-03-31 12:50:39.620121 stigg_api_client_v2-1.98.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      451 2024-03-31 12:50:39.620121 stigg_api_client_v2-1.98.0/stigg/generated/apply_subscription.py
--rw-r--r--   0        0        0      396 2024-03-31 12:50:39.620121 stigg_api_client_v2-1.98.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0    12593 2024-03-31 12:50:39.620121 stigg_api_client_v2-1.98.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0   131917 2024-03-31 12:50:39.620121 stigg_api_client_v2-1.98.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     6674 2024-03-31 12:50:39.620121 stigg_api_client_v2-1.98.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0      635 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      457 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      241 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0   131412 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/client.py
--rw-r--r--   0        0        0      457 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      523 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/detach_customer_payment_method.py
--rw-r--r--   0        0        0    28785 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      479 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      528 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2411 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    73593 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      513 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      409 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_checkout_state.py
--rw-r--r--   0        0        0      547 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      505 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      461 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      515 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_customer_statistics.py
--rw-r--r--   0        0        0      316 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      354 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      762 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      280 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      568 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      581 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      399 2024-03-31 12:50:39.624121 stigg_api_client_v2-1.98.0/stigg/generated/get_usage_history.py
--rw-r--r--   0        0        0      587 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/grant_promotional_entitlements.py
--rw-r--r--   0        0        0      403 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      284 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      297 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   170002 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      516 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0      475 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/preview_subscription.py
--rw-r--r--   0        0        0      451 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      491 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      298 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      260 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      377 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      455 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/report_usage_bulk.py
--rw-r--r--   0        0        0      478 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/revoke_promotional_entitlement.py
--rw-r--r--   0        0        0      473 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/transfer_subscription.py
--rw-r--r--   0        0        0      441 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/unarchive_customer.py
--rw-r--r--   0        0        0      403 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      457 2024-03-31 12:50:39.628121 stigg_api_client_v2-1.98.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 stigg_api_client_v2-1.98.0/PKG-INFO
+-rw-r--r--   0        0        0     5127 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/LICENSE
+-rw-r--r--   0        0        0     1644 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/README.md
+-rw-r--r--   0        0        0      549 2024-03-31 14:18:07.389409 stigg_api_client_v2-1.98.1/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/__init__.py
+-rw-r--r--   0        0        0    12780 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0    11617 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3521 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    24332 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     8481 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    30627 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     6266 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    26369 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0    13187 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      611 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    98560 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    22227 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      783 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_git.py
+-rw-r--r--   0        0        0      207 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0    16418 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0     5180 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_mock_val_ser.py
+-rw-r--r--   0        0        0    28114 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4568 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4855 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0     6293 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_signature.py
+-rw-r--r--   0        0        0    29094 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    17960 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12670 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     3226 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0    10054 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0    11913 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_migration.py
+-rw-r--r--   0        0        0     1600 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/alias_generators.py
+-rw-r--r--   0        0        0     4162 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/aliases.py
+-rw-r--r--   0        0        0     4357 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/annotated_handlers.py
+-rw-r--r--   0        0        0      147 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21493 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/color.py
+-rw-r--r--   0        0        0    29141 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/config.py
+-rw-r--r--   0        0        0    13450 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/dataclasses.py
+-rw-r--r--   0        0        0      149 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0      144 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/decorator.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9871 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     2663 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7595 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10778 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4580 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2511 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     3336 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0      147 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/env_settings.py
+-rw-r--r--   0        0        0      149 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4741 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/errors.py
+-rw-r--r--   0        0        0    45930 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/fields.py
+-rw-r--r--   0        0        0    14621 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    24317 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/functional_validators.py
+-rw-r--r--   0        0        0      143 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/generics.py
+-rw-r--r--   0        0        0      139 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/json.py
+-rw-r--r--   0        0        0   102809 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/json_schema.py
+-rw-r--r--   0        0        0    65892 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/main.py
+-rw-r--r--   0        0        0    55135 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/mypy.py
+-rw-r--r--   0        0        0    21225 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/networks.py
+-rw-r--r--   0        0        0      140 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/parse.py
+-rw-r--r--   0        0        0     6115 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0     1858 2024-03-31 14:17:00.084365 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/plugin/_loader.py
+-rw-r--r--   0        0        0     5228 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/plugin/_schema_validator.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/py.typed
+-rw-r--r--   0        0        0     5599 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/root_model.py
+-rw-r--r--   0        0        0      141 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/schema.py
+-rw-r--r--   0        0        0      140 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/tools.py
+-rw-r--r--   0        0        0    18108 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    89609 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/types.py
+-rw-r--r--   0        0        0      137 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/typing.py
+-rw-r--r--   0        0        0      140 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/utils.py
+-rw-r--r--   0        0        0     2771 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    15026 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6477 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/config.py
+-rw-r--r--   0        0        0    18073 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    14039 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5141 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50485 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17805 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44376 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38748 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    22059 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47614 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2826 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35379 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/types.py
+-rw-r--r--   0        0        0    18996 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21887 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1039 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/version.py
+-rw-r--r--   0        0        0     2054 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/validate_call_decorator.py
+-rw-r--r--   0        0        0      145 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/validators.py
+-rw-r--r--   0        0        0     2560 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/version.py
+-rw-r--r--   0        0        0     2322 2024-03-31 14:17:00.088364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/warnings.py
+-rw-r--r--   0        0        0        4 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0    85087 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/METADATA
+-rw-r--r--   0        0        0    14262 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/WHEEL
+-rw-r--r--   0        0        0     1129 2024-03-31 14:17:00.080364 stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     6886 2024-03-31 14:17:00.092365 stigg_api_client_v2-1.98.1/stigg/client.py
+-rw-r--r--   0        0        0     1455 2024-03-31 14:17:00.092365 stigg_api_client_v2-1.98.1/stigg/edge_utils.py
+-rw-r--r--   0        0        0    57896 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      451 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/apply_subscription.py
+-rw-r--r--   0        0        0      396 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0    12593 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0   132432 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     6674 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/base_client.py
+-rw-r--r--   0        0        0      635 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      457 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      241 2024-03-31 14:18:06.105389 stigg_api_client_v2-1.98.1/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0   131927 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/client.py
+-rw-r--r--   0        0        0      457 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      523 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/detach_customer_payment_method.py
+-rw-r--r--   0        0        0    28785 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/enums.py
+-rw-r--r--   0        0        0      479 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      528 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2411 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    74304 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      513 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      409 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_checkout_state.py
+-rw-r--r--   0        0        0      547 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      505 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      461 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      515 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_customer_statistics.py
+-rw-r--r--   0        0        0      316 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      354 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      762 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      280 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      568 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      581 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      399 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/get_usage_history.py
+-rw-r--r--   0        0        0      587 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/grant_promotional_entitlements.py
+-rw-r--r--   0        0        0      403 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      284 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      297 2024-03-31 14:18:06.109389 stigg_api_client_v2-1.98.1/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   170002 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      516 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0      475 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/preview_subscription.py
+-rw-r--r--   0        0        0      451 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      491 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      298 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      260 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      377 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      455 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/report_usage_bulk.py
+-rw-r--r--   0        0        0      478 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/revoke_promotional_entitlement.py
+-rw-r--r--   0        0        0      473 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/transfer_subscription.py
+-rw-r--r--   0        0        0      441 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/unarchive_customer.py
+-rw-r--r--   0        0        0      403 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      457 2024-03-31 14:18:06.113389 stigg_api_client_v2-1.98.1/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 stigg_api_client_v2-1.98.1/PKG-INFO
```

### Comparing `stigg_api_client_v2-1.98.0/LICENSE` & `stigg_api_client_v2-1.98.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/README.md` & `stigg_api_client_v2-1.98.1/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/pyproject.toml` & `stigg_api_client_v2-1.98.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "1.98.0"
+version = "1.98.1"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 license = "STIGG SDK LICENSE"
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
```

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/__init__.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_config.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_config.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_core_metadata.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_core_utils.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_core_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_dataclasses.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_decorators.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_decorators.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_decorators_v1.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_decorators_v1.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_discriminated_union.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_fields.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_fields.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_forward_ref.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_forward_ref.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_generate_schema.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_generate_schema.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_generics.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_generics.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_git.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_git.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_known_annotated_metadata.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_known_annotated_metadata.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_mock_val_ser.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_mock_val_ser.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_model_construction.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_model_construction.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_repr.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_repr.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_schema_generation_shared.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_schema_generation_shared.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_signature.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_signature.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_std_types_schema.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_std_types_schema.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_typing_extra.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_typing_extra.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_utils.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_validate_call.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_validate_call.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_internal/_validators.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_internal/_validators.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/_migration.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/_migration.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/alias_generators.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/alias_generators.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/aliases.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/aliases.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/annotated_handlers.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/annotated_handlers.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/color.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/color.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/config.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/dataclasses.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/dataclasses.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/class_validators.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/class_validators.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/config.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/config.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/copy_internals.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/decorator.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/json.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/parse.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/deprecated/tools.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/errors.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/fields.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/fields.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/functional_serializers.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/functional_serializers.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/functional_validators.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/functional_validators.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/json_schema.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/json_schema.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/main.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/main.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/mypy.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/mypy.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/networks.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/networks.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/plugin/__init__.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/plugin/_loader.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/plugin/_loader.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/plugin/_schema_validator.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/plugin/_schema_validator.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/root_model.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/root_model.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/type_adapter.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/type_adapter.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/types.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/__init__.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/_hypothesis_plugin.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/annotated_types.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/annotated_types.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/class_validators.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/class_validators.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/color.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/color.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/config.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/config.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/dataclasses.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/datetime_parse.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/decorator.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/decorator.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/env_settings.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/env_settings.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/error_wrappers.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/error_wrappers.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/errors.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/errors.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/fields.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/fields.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/generics.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/generics.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/json.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/json.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/main.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/main.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/mypy.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/mypy.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/networks.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/networks.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/parse.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/parse.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/schema.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/schema.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/tools.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/tools.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/types.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/types.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/typing.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/typing.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/utils.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/validators.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/validators.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/v1/version.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/v1/version.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/validate_call_decorator.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/validate_call_decorator.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/version.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/version.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic/warnings.py` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic/warnings.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/METADATA` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/RECORD` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/_vendors/pydantic-2.6.4.dist-info/licenses/LICENSE` & `stigg_api_client_v2-1.98.1/stigg/_vendors/pydantic-2.6.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/client.py` & `stigg_api_client_v2-1.98.1/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/edge_utils.py` & `stigg_api_client_v2-1.98.1/stigg/edge_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/__init__.py` & `stigg_api_client_v2-1.98.1/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,21 +235,24 @@
     ImmediateSubscriptionPreviewInvoiceFragmentProrationNetAmount,
     ImmediateSubscriptionPreviewInvoiceFragmentSubTotal,
     ImmediateSubscriptionPreviewInvoiceFragmentTax,
     ImmediateSubscriptionPreviewInvoiceFragmentTaxDetails,
     ImmediateSubscriptionPreviewInvoiceFragmentTotal,
     ImmediateSubscriptionPreviewInvoiceFragmentTotalExcludingTax,
     LayoutConfigurationFragment,
+    MockPaywallAddonDependencyFragment,
     MockPaywallAddonFragment,
+    MockPaywallAddonFragmentDependencies,
     MockPaywallAddonFragmentEntitlements,
     MockPaywallAddonFragmentPrices,
     MockPaywallPackageEntitlementFragment,
     MockPaywallPackageEntitlementFragmentFeature,
-    MockPaywallPackageGroupFragment,
-    MockPaywallPackageGroupFragmentCompatibleAddons,
+    MockPaywallPlanCompatiblePackageGroupsFragment,
+    MockPaywallPlanCompatiblePackageGroupsFragmentAddons,
+    MockPaywallPlanCompatiblePackageGroupsFragmentOptions,
     MockPaywallPlanFragment,
     MockPaywallPlanFragmentBasePlan,
     MockPaywallPlanFragmentCompatibleAddons,
     MockPaywallPlanFragmentCompatiblePackageGroups,
     MockPaywallPlanFragmentDefaultTrialConfig,
     MockPaywallPlanFragmentEntitlements,
     MockPaywallPlanFragmentInheritedEntitlements,
@@ -1165,21 +1168,24 @@
     "MeterAggregation",
     "MeterConditionInput",
     "MeterFilterDefinitionInput",
     "MeterType",
     "MeterTypeFilterComparison",
     "MigrateSubscriptionToLatest",
     "MigrateSubscriptionToLatestMigrateSubscriptionToLatest",
+    "MockPaywallAddonDependencyFragment",
     "MockPaywallAddonFragment",
+    "MockPaywallAddonFragmentDependencies",
     "MockPaywallAddonFragmentEntitlements",
     "MockPaywallAddonFragmentPrices",
     "MockPaywallPackageEntitlementFragment",
     "MockPaywallPackageEntitlementFragmentFeature",
-    "MockPaywallPackageGroupFragment",
-    "MockPaywallPackageGroupFragmentCompatibleAddons",
+    "MockPaywallPlanCompatiblePackageGroupsFragment",
+    "MockPaywallPlanCompatiblePackageGroupsFragmentAddons",
+    "MockPaywallPlanCompatiblePackageGroupsFragmentOptions",
     "MockPaywallPlanFragment",
     "MockPaywallPlanFragmentBasePlan",
     "MockPaywallPlanFragmentCompatibleAddons",
     "MockPaywallPlanFragmentCompatiblePackageGroups",
     "MockPaywallPlanFragmentDefaultTrialConfig",
     "MockPaywallPlanFragmentEntitlements",
     "MockPaywallPlanFragmentInheritedEntitlements",
```

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-1.98.1/stigg/generated/async_base_client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/async_client.py` & `stigg_api_client_v2-1.98.1/stigg/generated/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,14 +799,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -2353,14 +2354,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -2762,14 +2764,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -3278,14 +3281,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -4233,14 +4237,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -4562,21 +4567,30 @@
             fragment LayoutConfigurationFragment on PaywallLayoutConfiguration {
               alignment
               planWidth
               planMargin
               planPadding
             }
 
+            fragment MockPaywallAddonDependencyFragment on PaywallAddon {
+              refId
+              displayName
+              description
+            }
+
             fragment MockPaywallAddonFragment on PaywallAddon {
               refId
               displayName
               description
               additionalMetaData
               billingId
               maxQuantity
+              dependencies {
+                ...MockPaywallAddonDependencyFragment
+              }
               entitlements {
                 ...MockPaywallPackageEntitlementFragment
               }
               prices {
                 ...MockPaywallPriceFragment
               }
               pricingType
@@ -4597,21 +4611,25 @@
                 displayName
                 description
                 refId
                 additionalMetaData
               }
             }
 
-            fragment MockPaywallPackageGroupFragment on PaywallPackageGroup {
+            fragment MockPaywallPlanCompatiblePackageGroupsFragment on PaywallPlanCompatiblePackageGroup {
               packageGroupId
               displayName
               description
-              compatibleAddons {
+              addons {
                 ...MockPaywallAddonFragment
               }
+              options {
+                minItems
+                freeItems
+              }
             }
 
             fragment MockPaywallPlanFragment on PaywallPlan {
               refId
               description
               displayName
               billingId
@@ -4640,15 +4658,15 @@
                 duration
                 units
               }
               compatibleAddons {
                 ...MockPaywallAddonFragment
               }
               compatiblePackageGroups {
-                ...MockPaywallPackageGroupFragment
+                ...MockPaywallPlanCompatiblePackageGroupsFragment
               }
             }
 
             fragment MockPaywallPriceFragment on PaywallPrice {
               billingModel
               billingPeriod
               billingId
```

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/base_client.py` & `stigg_api_client_v2-1.98.1/stigg/generated/base_client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/base_model.py` & `stigg_api_client_v2-1.98.1/stigg/generated/base_model.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/client.py` & `stigg_api_client_v2-1.98.1/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -799,14 +799,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -2351,14 +2352,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -2760,14 +2762,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -3276,14 +3279,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -4231,14 +4235,15 @@
               packageGroupId
               displayName
               addons {
                 ...AddonFragment
               }
               options {
                 minItems
+                freeItems
               }
             }
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
@@ -4558,21 +4563,30 @@
             fragment LayoutConfigurationFragment on PaywallLayoutConfiguration {
               alignment
               planWidth
               planMargin
               planPadding
             }
 
+            fragment MockPaywallAddonDependencyFragment on PaywallAddon {
+              refId
+              displayName
+              description
+            }
+
             fragment MockPaywallAddonFragment on PaywallAddon {
               refId
               displayName
               description
               additionalMetaData
               billingId
               maxQuantity
+              dependencies {
+                ...MockPaywallAddonDependencyFragment
+              }
               entitlements {
                 ...MockPaywallPackageEntitlementFragment
               }
               prices {
                 ...MockPaywallPriceFragment
               }
               pricingType
@@ -4593,21 +4607,25 @@
                 displayName
                 description
                 refId
                 additionalMetaData
               }
             }
 
-            fragment MockPaywallPackageGroupFragment on PaywallPackageGroup {
+            fragment MockPaywallPlanCompatiblePackageGroupsFragment on PaywallPlanCompatiblePackageGroup {
               packageGroupId
               displayName
               description
-              compatibleAddons {
+              addons {
                 ...MockPaywallAddonFragment
               }
+              options {
+                minItems
+                freeItems
+              }
             }
 
             fragment MockPaywallPlanFragment on PaywallPlan {
               refId
               description
               displayName
               billingId
@@ -4636,15 +4654,15 @@
                 duration
                 units
               }
               compatibleAddons {
                 ...MockPaywallAddonFragment
               }
               compatiblePackageGroups {
-                ...MockPaywallPackageGroupFragment
+                ...MockPaywallPlanCompatiblePackageGroupsFragment
               }
             }
 
             fragment MockPaywallPriceFragment on PaywallPrice {
               billingModel
               billingPeriod
               billingId
```

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/detach_customer_payment_method.py` & `stigg_api_client_v2-1.98.1/stigg/generated/detach_customer_payment_method.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/enums.py` & `stigg_api_client_v2-1.98.1/stigg/generated/enums.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-1.98.1/stigg/generated/estimate_subscription_update.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-1.98.1/stigg/generated/exceptions.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/fragments.py` & `stigg_api_client_v2-1.98.1/stigg/generated/fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,66 +87,66 @@
 
 
 class PriceTierFragmentFlatPrice(BaseModel):
     amount: float
     currency: Currency
 
 
-class PriceFragment(BaseModel):
+class OveragePriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
-    billing_cadence: BillingCadence = Field(alias="billingCadence")
     billing_id: Optional[str] = Field(alias="billingId")
-    min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
-    max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
-    price: Optional["PriceFragmentPrice"]
+    price: Optional["OveragePriceFragmentPrice"]
     tiers_mode: Optional[TiersMode] = Field(alias="tiersMode")
-    tiers: Optional[List["PriceFragmentTiers"]]
-    feature: Optional["PriceFragmentFeature"]
+    tiers: Optional[List["OveragePriceFragmentTiers"]]
+    feature: Optional["OveragePriceFragmentFeature"]
 
 
-class PriceFragmentPrice(BaseModel):
+class OveragePriceFragmentPrice(BaseModel):
     amount: float
     currency: Currency
 
 
-class PriceFragmentTiers(PriceTierFragment):
+class OveragePriceFragmentTiers(PriceTierFragment):
     pass
 
 
-class PriceFragmentFeature(BaseModel):
+class OveragePriceFragmentFeature(BaseModel):
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
-class OveragePriceFragment(BaseModel):
+class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
+    billing_cadence: BillingCadence = Field(alias="billingCadence")
     billing_id: Optional[str] = Field(alias="billingId")
+    min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
+    max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
-    price: Optional["OveragePriceFragmentPrice"]
+    price: Optional["PriceFragmentPrice"]
     tiers_mode: Optional[TiersMode] = Field(alias="tiersMode")
-    tiers: Optional[List["OveragePriceFragmentTiers"]]
-    feature: Optional["OveragePriceFragmentFeature"]
+    tiers: Optional[List["PriceFragmentTiers"]]
+    feature: Optional["PriceFragmentFeature"]
 
 
-class OveragePriceFragmentPrice(BaseModel):
+class PriceFragmentPrice(BaseModel):
     amount: float
     currency: Currency
 
 
-class OveragePriceFragmentTiers(PriceTierFragment):
+class PriceFragmentTiers(PriceTierFragment):
     pass
 
 
-class OveragePriceFragmentFeature(BaseModel):
+class PriceFragmentFeature(BaseModel):
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
@@ -179,38 +179,88 @@
     pass
 
 
 class AddonFragmentDependencies(AddonDependencyFragment):
     pass
 
 
-class SubscriptionInvoiceFragment(BaseModel):
-    billing_id: str = Field(alias="billingId")
-    status: SubscriptionInvoiceStatus
-    created_at: Any = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    requires_action: bool = Field(alias="requiresAction")
-    payment_url: Optional[str] = Field(alias="paymentUrl")
-    payment_secret: Optional[str] = Field(alias="paymentSecret")
-    error_message: Optional[str] = Field(alias="errorMessage")
+class FeatureFragment(BaseModel):
+    typename__: str = Field(alias="__typename")
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    ref_id: str = Field(alias="refId")
 
 
-class PlanCompatiblePackageGroupsFragment(BaseModel):
-    package_group_id: str = Field(alias="packageGroupId")
-    display_name: str = Field(alias="displayName")
-    addons: Optional[List["PlanCompatiblePackageGroupsFragmentAddons"]]
-    options: "PlanCompatiblePackageGroupsFragmentOptions"
+class EntitlementFragment(BaseModel):
+    typename__: str = Field(alias="__typename")
+    is_granted: bool = Field(alias="isGranted")
+    access_denied_reason: Optional[AccessDeniedReason] = Field(
+        alias="accessDeniedReason"
+    )
+    customer_id: Optional[str] = Field(alias="customerId")
+    resource_id: Optional[str] = Field(alias="resourceId")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    has_soft_limit: Optional[bool] = Field(alias="hasSoftLimit")
+    current_usage: Optional[float] = Field(alias="currentUsage")
+    requested_usage: Optional[float] = Field(alias="requestedUsage")
+    entitlement_updated_at: Optional[Any] = Field(alias="entitlementUpdatedAt")
+    usage_updated_at: Optional[Any] = Field(alias="usageUpdatedAt")
+    next_reset_date: Optional[Any] = Field(alias="nextResetDate")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    reset_period_configuration: Optional[
+        Annotated[
+            Union[
+                "EntitlementFragmentResetPeriodConfigurationMonthlyResetPeriodConfig",
+                "EntitlementFragmentResetPeriodConfigurationWeeklyResetPeriodConfig",
+                "EntitlementFragmentResetPeriodConfigurationYearlyResetPeriodConfig",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="resetPeriodConfiguration")
+    feature: Optional["EntitlementFragmentFeature"]
 
 
-class PlanCompatiblePackageGroupsFragmentAddons(AddonFragment):
+class EntitlementFragmentResetPeriodConfigurationMonthlyResetPeriodConfig(BaseModel):
+    typename__: Literal["MonthlyResetPeriodConfig"] = Field(alias="__typename")
+    monthly_according_to: Optional[MonthlyAccordingTo] = Field(
+        alias="monthlyAccordingTo"
+    )
+
+
+class EntitlementFragmentResetPeriodConfigurationWeeklyResetPeriodConfig(BaseModel):
+    typename__: Literal["WeeklyResetPeriodConfig"] = Field(alias="__typename")
+    weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
+
+
+class EntitlementFragmentResetPeriodConfigurationYearlyResetPeriodConfig(BaseModel):
+    typename__: Literal["YearlyResetPeriodConfig"] = Field(alias="__typename")
+
+
+class EntitlementFragmentFeature(FeatureFragment):
     pass
 
 
-class PlanCompatiblePackageGroupsFragmentOptions(BaseModel):
-    min_items: Optional[float] = Field(alias="minItems")
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
 
 
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -224,14 +274,30 @@
 
 
 class ProductFragmentProductSettingsDowngradePlan(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
 
 
+class PlanCompatiblePackageGroupsFragment(BaseModel):
+    package_group_id: str = Field(alias="packageGroupId")
+    display_name: str = Field(alias="displayName")
+    addons: Optional[List["PlanCompatiblePackageGroupsFragmentAddons"]]
+    options: "PlanCompatiblePackageGroupsFragmentOptions"
+
+
+class PlanCompatiblePackageGroupsFragmentAddons(AddonFragment):
+    pass
+
+
+class PlanCompatiblePackageGroupsFragmentOptions(BaseModel):
+    min_items: Optional[float] = Field(alias="minItems")
+    free_items: Optional[float] = Field(alias="freeItems")
+
+
 class PlanFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     billing_id: Optional[str] = Field(alias="billingId")
     version_number: int = Field(alias="versionNumber")
@@ -293,18 +359,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class SubscriptionFutureUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
@@ -515,27 +577,27 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
+class SubscriptionInvoiceFragment(BaseModel):
+    billing_id: str = Field(alias="billingId")
+    status: SubscriptionInvoiceStatus
+    created_at: Any = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    requires_action: bool = Field(alias="requiresAction")
+    payment_url: Optional[str] = Field(alias="paymentUrl")
+    payment_secret: Optional[str] = Field(alias="paymentSecret")
+    error_message: Optional[str] = Field(alias="errorMessage")
 
 
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
 
 
 class SubscriptionFragment(BaseModel):
     id: str
     subscription_id: str = Field(alias="subscriptionId")
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -616,75 +678,14 @@
     pass
 
 
 class SubscriptionFragmentFutureUpdates(SubscriptionFutureUpdateData):
     pass
 
 
-class FeatureFragment(BaseModel):
-    typename__: str = Field(alias="__typename")
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    ref_id: str = Field(alias="refId")
-
-
-class EntitlementFragment(BaseModel):
-    typename__: str = Field(alias="__typename")
-    is_granted: bool = Field(alias="isGranted")
-    access_denied_reason: Optional[AccessDeniedReason] = Field(
-        alias="accessDeniedReason"
-    )
-    customer_id: Optional[str] = Field(alias="customerId")
-    resource_id: Optional[str] = Field(alias="resourceId")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    has_soft_limit: Optional[bool] = Field(alias="hasSoftLimit")
-    current_usage: Optional[float] = Field(alias="currentUsage")
-    requested_usage: Optional[float] = Field(alias="requestedUsage")
-    entitlement_updated_at: Optional[Any] = Field(alias="entitlementUpdatedAt")
-    usage_updated_at: Optional[Any] = Field(alias="usageUpdatedAt")
-    next_reset_date: Optional[Any] = Field(alias="nextResetDate")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    reset_period_configuration: Optional[
-        Annotated[
-            Union[
-                "EntitlementFragmentResetPeriodConfigurationMonthlyResetPeriodConfig",
-                "EntitlementFragmentResetPeriodConfigurationWeeklyResetPeriodConfig",
-                "EntitlementFragmentResetPeriodConfigurationYearlyResetPeriodConfig",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="resetPeriodConfiguration")
-    feature: Optional["EntitlementFragmentFeature"]
-
-
-class EntitlementFragmentResetPeriodConfigurationMonthlyResetPeriodConfig(BaseModel):
-    typename__: Literal["MonthlyResetPeriodConfig"] = Field(alias="__typename")
-    monthly_according_to: Optional[MonthlyAccordingTo] = Field(
-        alias="monthlyAccordingTo"
-    )
-
-
-class EntitlementFragmentResetPeriodConfigurationWeeklyResetPeriodConfig(BaseModel):
-    typename__: Literal["WeeklyResetPeriodConfig"] = Field(alias="__typename")
-    weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
-
-
-class EntitlementFragmentResetPeriodConfigurationYearlyResetPeriodConfig(BaseModel):
-    typename__: Literal["YearlyResetPeriodConfig"] = Field(alias="__typename")
-
-
-class EntitlementFragmentFeature(FeatureFragment):
-    pass
-
-
 class ApplySubscriptionFragment(BaseModel):
     subscription: Optional["ApplySubscriptionFragmentSubscription"]
     entitlements: Optional[List["ApplySubscriptionFragmentEntitlements"]]
 
 
 class ApplySubscriptionFragmentSubscription(SubscriptionFragment):
     pass
@@ -744,37 +745,14 @@
     typename__: Literal["TypographyConfiguration"] = Field(alias="__typename")
 
 
 class CheckoutConfigurationFragmentContent(BaseModel):
     collect_phone_number: Optional[bool] = Field(alias="collectPhoneNumber")
 
 
-class PromotionalEntitlementFragment(BaseModel):
-    status: PromotionalEntitlementStatus
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    feature_id: str = Field(alias="featureId")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    has_soft_limit: Optional[bool] = Field(alias="hasSoftLimit")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    end_date: Optional[Any] = Field(alias="endDate")
-    is_visible: bool = Field(alias="isVisible")
-    feature: "PromotionalEntitlementFragmentFeature"
-
-
-class PromotionalEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class CouponFragment(BaseModel):
     id: str
     discount_value: float = Field(alias="discountValue")
     type: CouponType
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     ref_id: str = Field(alias="refId")
     name: str
@@ -806,14 +784,37 @@
     ref_id: str = Field(alias="refId")
     customer_id: str = Field(alias="customerId")
     billing_id: Optional[str] = Field(alias="billingId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     aws_marketplace_customer_id: Optional[str] = Field(alias="awsMarketplaceCustomerId")
 
 
+class PromotionalEntitlementFragment(BaseModel):
+    status: PromotionalEntitlementStatus
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    feature_id: str = Field(alias="featureId")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    has_soft_limit: Optional[bool] = Field(alias="hasSoftLimit")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    end_date: Optional[Any] = Field(alias="endDate")
+    is_visible: bool = Field(alias="isVisible")
+    feature: "PromotionalEntitlementFragmentFeature"
+
+
+class PromotionalEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -987,22 +988,39 @@
     typename__: Literal["YearlyResetPeriodConfig"] = Field(alias="__typename")
 
 
 class CustomerPortalEntitlementFragmentFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlementFragment(BaseModel):
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
+
+
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    has_soft_limit: Optional[bool] = Field(alias="hasSoftLimit")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+
+
+class CustomerPortalSubscriptionAddonFragment(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
 
 
 class CustomerPortalSubscriptionScheduledUpdateDataFragment(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -1115,41 +1133,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionPriceFragment(BaseModel):
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    billing_model: Optional[BillingModel] = Field(alias="billingModel")
-    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
-    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
-
-
-class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-
-
-class CustomerPortalSubscriptionAddonFragment(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -1227,14 +1218,24 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateDataFragment
 ):
     pass
 
 
+class CustomerPortalPromotionalEntitlementFragment(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    has_soft_limit: Optional[bool] = Field(alias="hasSoftLimit")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -1436,14 +1437,20 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
+class MockPaywallAddonDependencyFragment(BaseModel):
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+
+
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -1493,40 +1500,49 @@
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     max_quantity: Optional[float] = Field(alias="maxQuantity")
+    dependencies: Optional[List["MockPaywallAddonFragmentDependencies"]]
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
     prices: List["MockPaywallAddonFragmentPrices"]
     pricing_type: Optional[PricingType] = Field(alias="pricingType")
 
 
+class MockPaywallAddonFragmentDependencies(MockPaywallAddonDependencyFragment):
+    pass
+
+
 class MockPaywallAddonFragmentEntitlements(MockPaywallPackageEntitlementFragment):
     pass
 
 
 class MockPaywallAddonFragmentPrices(MockPaywallPriceFragment):
     pass
 
 
-class MockPaywallPackageGroupFragment(BaseModel):
+class MockPaywallPlanCompatiblePackageGroupsFragment(BaseModel):
     package_group_id: str = Field(alias="packageGroupId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
-    compatible_addons: Optional[
-        List["MockPaywallPackageGroupFragmentCompatibleAddons"]
-    ] = Field(alias="compatibleAddons")
+    addons: Optional[List["MockPaywallPlanCompatiblePackageGroupsFragmentAddons"]]
+    options: "MockPaywallPlanCompatiblePackageGroupsFragmentOptions"
 
 
-class MockPaywallPackageGroupFragmentCompatibleAddons(MockPaywallAddonFragment):
+class MockPaywallPlanCompatiblePackageGroupsFragmentAddons(MockPaywallAddonFragment):
     pass
 
 
+class MockPaywallPlanCompatiblePackageGroupsFragmentOptions(BaseModel):
+    min_items: Optional[float] = Field(alias="minItems")
+    free_items: Optional[float] = Field(alias="freeItems")
+
+
 class MockPaywallPlanFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     billing_id: Optional[str] = Field(alias="billingId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product: "MockPaywallPlanFragmentProduct"
@@ -1579,15 +1595,17 @@
     units: TrialPeriodUnits
 
 
 class MockPaywallPlanFragmentCompatibleAddons(MockPaywallAddonFragment):
     pass
 
 
-class MockPaywallPlanFragmentCompatiblePackageGroups(MockPaywallPackageGroupFragment):
+class MockPaywallPlanFragmentCompatiblePackageGroups(
+    MockPaywallPlanCompatiblePackageGroupsFragment
+):
     pass
 
 
 class PackagePublishedPayload(BaseModel):
     account_id: str = Field(alias="accountId")
     environment_id: str = Field(alias="environmentId")
     package_type: str = Field(alias="packageType")
@@ -2073,57 +2091,58 @@
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
 AddonDependencyFragment.model_rebuild()
 PackageEntitlementFragment.model_rebuild()
 PriceTierFragment.model_rebuild()
-PriceFragment.model_rebuild()
 OveragePriceFragment.model_rebuild()
+PriceFragment.model_rebuild()
 AddonFragment.model_rebuild()
-SubscriptionInvoiceFragment.model_rebuild()
-PlanCompatiblePackageGroupsFragment.model_rebuild()
+FeatureFragment.model_rebuild()
+EntitlementFragment.model_rebuild()
+TotalPriceFragment.model_rebuild()
 ProductFragment.model_rebuild()
+PlanCompatiblePackageGroupsFragment.model_rebuild()
 PlanFragment.model_rebuild()
-CustomerResourceFragment.model_rebuild()
 SubscriptionFutureUpdateData.model_rebuild()
 SubscriptionScheduledUpdateData.model_rebuild()
-TotalPriceFragment.model_rebuild()
+SubscriptionInvoiceFragment.model_rebuild()
+CustomerResourceFragment.model_rebuild()
 SubscriptionFragment.model_rebuild()
-FeatureFragment.model_rebuild()
-EntitlementFragment.model_rebuild()
 ApplySubscriptionFragment.model_rebuild()
 FontVariantFragment.model_rebuild()
 TypographyConfigurationFragment.model_rebuild()
 CheckoutConfigurationFragment.model_rebuild()
-PromotionalEntitlementFragment.model_rebuild()
 CouponFragment.model_rebuild()
 SlimCustomerFragment.model_rebuild()
+PromotionalEntitlementFragment.model_rebuild()
 CustomerFragment.model_rebuild()
 CheckoutStateFragment.model_rebuild()
 CustomerPortalBillingInformationFragment.model_rebuild()
 CustomerPortalConfigurationFragment.model_rebuild()
 CustomerPortalEntitlementFragment.model_rebuild()
-CustomerPortalPromotionalEntitlementFragment.model_rebuild()
-CustomerPortalSubscriptionScheduledUpdateDataFragment.model_rebuild()
 CustomerPortalSubscriptionPriceFragment.model_rebuild()
 CustomerPortalSubscriptionAddonFragment.model_rebuild()
+CustomerPortalSubscriptionScheduledUpdateDataFragment.model_rebuild()
 CustomerPortalSubscriptionFragment.model_rebuild()
+CustomerPortalPromotionalEntitlementFragment.model_rebuild()
 CustomerPortalFragment.model_rebuild()
 CustomerStatisticsFragment.model_rebuild()
 CustomerWithSubscriptionsFragment.model_rebuild()
 UsageUpdatedFragment.model_rebuild()
 EntitlementUsageUpdated.model_rebuild()
 EntitlementsUpdatedPayload.model_rebuild()
 ImmediateSubscriptionPreviewInvoiceFragment.model_rebuild()
 LayoutConfigurationFragment.model_rebuild()
+MockPaywallAddonDependencyFragment.model_rebuild()
 MockPaywallPriceFragment.model_rebuild()
 MockPaywallPackageEntitlementFragment.model_rebuild()
 MockPaywallAddonFragment.model_rebuild()
-MockPaywallPackageGroupFragment.model_rebuild()
+MockPaywallPlanCompatiblePackageGroupsFragment.model_rebuild()
 MockPaywallPlanFragment.model_rebuild()
 PackagePublishedPayload.model_rebuild()
 PaywallCalculatedPricePointsFragment.model_rebuild()
 PaywallConfigurationFragment.model_rebuild()
 PaywallCurrencyFragment.model_rebuild()
 PaywallFragment.model_rebuild()
 SlimSubscriptionFragment.model_rebuild()
```

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-1.98.1/stigg/generated/get_active_subscriptions.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-1.98.1/stigg/generated/get_coupons.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/get_customer_statistics.py` & `stigg_api_client_v2-1.98.1/stigg/generated/get_customer_statistics.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-1.98.1/stigg/generated/get_mock_paywall.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/get_products.py` & `stigg_api_client_v2-1.98.1/stigg/generated/get_products.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-1.98.1/stigg/generated/get_sdk_configuration.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/grant_promotional_entitlements.py` & `stigg_api_client_v2-1.98.1/stigg/generated/grant_promotional_entitlements.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/input_types.py` & `stigg_api_client_v2-1.98.1/stigg/generated/input_types.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-1.98.1/stigg/generated/migrate_subscription_to_latest.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-1.98.0/PKG-INFO` & `stigg_api_client_v2-1.98.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 1.98.0
+Version: 1.98.1
 Summary: 
 License: STIGG SDK LICENSE
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

