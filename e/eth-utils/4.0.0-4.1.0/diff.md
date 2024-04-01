# Comparing `tmp/eth-utils-4.0.0.tar.gz` & `tmp/eth-utils-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-utils-4.0.0.tar", last modified: Thu Feb 22 20:39:59 2024, max compression
+gzip compressed data, was "eth-utils-4.1.0.tar", last modified: Mon Apr  1 19:54:24 2024, max compression
```

## Comparing `eth-utils-4.0.0.tar` & `eth-utils-4.1.0.tar`

### file list

```diff
@@ -1,101 +1,100 @@
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.810598 eth-utils-4.0.0/
--rw-r--r--   0 reedsa     (501) staff       (20)     1095 2024-02-20 17:40:35.000000 eth-utils-4.0.0/LICENSE
--rw-r--r--   0 reedsa     (501) staff       (20)      211 2024-02-20 17:41:21.000000 eth-utils-4.0.0/MANIFEST.in
--rw-r--r--   0 reedsa     (501) staff       (20)     5207 2024-02-22 20:39:59.795044 eth-utils-4.0.0/PKG-INFO
--rw-r--r--   0 reedsa     (501) staff       (20)     3086 2024-02-20 17:41:21.000000 eth-utils-4.0.0/README.md
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.710462 eth-utils-4.0.0/eth_utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     2343 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/__init__.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.719500 eth-utils-4.0.0/eth_utils/__json/
--rw-r--r--   0 reedsa     (501) staff       (20)   304350 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/__json/eth_networks.json
--rw-r--r--   0 reedsa     (501) staff       (20)       86 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/__main__.py
--rw-r--r--   0 reedsa     (501) staff       (20)     2050 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/abi.py
--rw-r--r--   0 reedsa     (501) staff       (20)     4218 2024-02-22 20:34:00.000000 eth-utils-4.0.0/eth_utils/address.py
--rw-r--r--   0 reedsa     (501) staff       (20)     4342 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/applicators.py
--rw-r--r--   0 reedsa     (501) staff       (20)     5500 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/conversions.py
--rw-r--r--   0 reedsa     (501) staff       (20)      362 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/crypto.py
--rw-r--r--   0 reedsa     (501) staff       (20)     3021 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/currency.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.721140 eth-utils-4.0.0/eth_utils/curried/
--rw-r--r--   0 reedsa     (501) staff       (20)     6497 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/curried/__init__.py
--rw-r--r--   0 reedsa     (501) staff       (20)      499 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/debug.py
--rw-r--r--   0 reedsa     (501) staff       (20)     3997 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/decorators.py
--rw-r--r--   0 reedsa     (501) staff       (20)      199 2024-02-20 17:40:35.000000 eth-utils-4.0.0/eth_utils/encoding.py
--rw-r--r--   0 reedsa     (501) staff       (20)      110 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/exceptions.py
--rw-r--r--   0 reedsa     (501) staff       (20)     2100 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/functional.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1828 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/hexadecimal.py
--rw-r--r--   0 reedsa     (501) staff       (20)     4148 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/humanize.py
--rw-r--r--   0 reedsa     (501) staff       (20)     5155 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/logging.py
--rw-r--r--   0 reedsa     (501) staff       (20)      842 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/module_loading.py
--rw-r--r--   0 reedsa     (501) staff       (20)     2244 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/network.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1190 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/numeric.py
--rw-r--r--   0 reedsa     (501) staff       (20)        0 2024-02-20 17:40:35.000000 eth-utils-4.0.0/eth_utils/py.typed
--rw-r--r--   0 reedsa     (501) staff       (20)     2617 2024-02-20 17:40:35.000000 eth-utils-4.0.0/eth_utils/toolz.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1074 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/types.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.722470 eth-utils-4.0.0/eth_utils/typing/
--rw-r--r--   0 reedsa     (501) staff       (20)      325 2024-02-20 17:40:35.000000 eth-utils-4.0.0/eth_utils/typing/__init__.py
--rw-r--r--   0 reedsa     (501) staff       (20)      190 2024-02-20 17:41:21.000000 eth-utils-4.0.0/eth_utils/typing/misc.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1757 2024-02-20 17:40:35.000000 eth-utils-4.0.0/eth_utils/units.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.781294 eth-utils-4.0.0/eth_utils.egg-info/
--rw-r--r--   0 reedsa     (501) staff       (20)     5207 2024-02-22 20:39:59.000000 eth-utils-4.0.0/eth_utils.egg-info/PKG-INFO
--rw-r--r--   0 reedsa     (501) staff       (20)     2467 2024-02-22 20:39:59.000000 eth-utils-4.0.0/eth_utils.egg-info/SOURCES.txt
--rw-r--r--   0 reedsa     (501) staff       (20)        1 2024-02-22 20:39:59.000000 eth-utils-4.0.0/eth_utils.egg-info/dependency_links.txt
--rw-r--r--   0 reedsa     (501) staff       (20)        1 2024-02-20 17:42:08.000000 eth-utils-4.0.0/eth_utils.egg-info/not-zip-safe
--rw-r--r--   0 reedsa     (501) staff       (20)      555 2024-02-22 20:39:59.000000 eth-utils-4.0.0/eth_utils.egg-info/requires.txt
--rw-r--r--   0 reedsa     (501) staff       (20)       10 2024-02-22 20:39:59.000000 eth-utils-4.0.0/eth_utils.egg-info/top_level.txt
--rw-r--r--   0 reedsa     (501) staff       (20)     3419 2024-02-20 17:41:21.000000 eth-utils-4.0.0/pyproject.toml
--rw-r--r--   0 reedsa     (501) staff       (20)       38 2024-02-22 20:39:59.810797 eth-utils-4.0.0/setup.cfg
--rw-r--r--   0 reedsa     (501) staff       (20)     2182 2024-02-22 20:39:52.000000 eth-utils-4.0.0/setup.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.723233 eth-utils-4.0.0/tests/
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.733545 eth-utils-4.0.0/tests/abi-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     5031 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/abi-utils/test_abi_utils.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.742740 eth-utils-4.0.0/tests/address-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)    10843 2024-02-22 20:34:00.000000 eth-utils-4.0.0/tests/address-utils/test_address_utils.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.743602 eth-utils-4.0.0/tests/applicator-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     6721 2024-02-20 17:40:35.000000 eth-utils-4.0.0/tests/applicator-utils/test_applicators.py
--rw-r--r--   0 reedsa     (501) staff       (20)      121 2024-02-20 17:40:35.000000 eth-utils-4.0.0/tests/conftest.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.744217 eth-utils-4.0.0/tests/conversion-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     4567 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/conversion-utils/test_conversions.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.744841 eth-utils-4.0.0/tests/core/
--rw-r--r--   0 reedsa     (501) staff       (20)       91 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/core/test_import_and_version.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.746958 eth-utils-4.0.0/tests/currency-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     4393 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/currency-utils/test_currency_tools.py
--rw-r--r--   0 reedsa     (501) staff       (20)      193 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/currency-utils/test_denoms_obj.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.747760 eth-utils-4.0.0/tests/curried-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     3223 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/curried-utils/test_curried.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.751188 eth-utils-4.0.0/tests/decorator-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)      666 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/decorator-utils/test_combomethod.py
--rw-r--r--   0 reedsa     (501) staff       (20)      690 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/decorator-utils/test_replace_exceptions.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1531 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/decorator-utils/test_validate_conversion_arguments.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.751892 eth-utils-4.0.0/tests/encoding-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     1083 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/encoding-utils/test_big_endian_integer.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.753414 eth-utils-4.0.0/tests/functional-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     1475 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/functional-utils/test_return_value_decorators.py
--rw-r--r--   0 reedsa     (501) staff       (20)     2569 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/functional-utils/test_type_inference.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.759958 eth-utils-4.0.0/tests/hexadecimal-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     1076 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/hexadecimal-utils/test_0x_prefix_addition_and_removal.py
--rw-r--r--   0 reedsa     (501) staff       (20)      487 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/hexadecimal-utils/test_is_0x_prefixed.py
--rw-r--r--   0 reedsa     (501) staff       (20)      972 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/hexadecimal-utils/test_is_hex.py
--rw-r--r--   0 reedsa     (501) staff       (20)      954 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/hexadecimal-utils/test_is_hexstr.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.764293 eth-utils-4.0.0/tests/humanize-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)      374 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/humanize-utils/test_humanize_bytes.py
--rw-r--r--   0 reedsa     (501) staff       (20)      230 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/humanize-utils/test_humanize_hash.py
--rw-r--r--   0 reedsa     (501) staff       (20)      714 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/humanize-utils/test_humanize_integer_sequence.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1202 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/humanize-utils/test_humanize_ipfs_uri.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1416 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/humanize-utils/test_humanize_seconds.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1608 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/humanize-utils/test_humanize_wei.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.768701 eth-utils-4.0.0/tests/logging-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     2919 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/logging-utils/test_DEBUG2_logging.py
--rw-r--r--   0 reedsa     (501) staff       (20)      630 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/logging-utils/test_compat_with_abc_ABC.py
--rw-r--r--   0 reedsa     (501) staff       (20)     2472 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/logging-utils/test_get_logger.py
--rw-r--r--   0 reedsa     (501) staff       (20)     2760 2024-02-20 17:40:35.000000 eth-utils-4.0.0/tests/logging-utils/test_has_logger_metaclass.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.769558 eth-utils-4.0.0/tests/module-loading-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)      266 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/module-loading-utils/test_import_string.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.770155 eth-utils-4.0.0/tests/network-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     2053 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/network-utils/test_network_utils.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.770927 eth-utils-4.0.0/tests/numeric-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)      369 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/numeric-utils/test_clamp.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.774594 eth-utils-4.0.0/tests/type-checks/
--rw-r--r--   0 reedsa     (501) staff       (20)     2216 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/type-checks/mypy_typing_of_curried_utils.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1927 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/type-checks/mypy_typing_of_functional_utils.py
--rw-r--r--   0 reedsa     (501) staff       (20)     1352 2024-02-20 17:41:21.000000 eth-utils-4.0.0/tests/type-checks/mypy_typing_of_has_logger.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-02-22 20:39:59.776766 eth-utils-4.0.0/tests/types-utils/
--rw-r--r--   0 reedsa     (501) staff       (20)     3014 2024-02-20 17:40:35.000000 eth-utils-4.0.0/tests/types-utils/test_types_utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.939384 eth-utils-4.1.0/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2023-05-01 17:17:17.000000 eth-utils-4.1.0/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      211 2024-01-09 21:45:03.000000 eth-utils-4.1.0/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5193 2024-04-01 19:54:24.939384 eth-utils-4.1.0/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3086 2024-01-09 21:45:03.000000 eth-utils-4.1.0/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2343 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/__json/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)   304350 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/__json/eth_networks.json
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       86 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/__main__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2050 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/abi.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4218 2024-03-25 20:53:18.000000 eth-utils-4.1.0/eth_utils/address.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4342 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/applicators.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5500 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/conversions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      362 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/crypto.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3021 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/currency.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/curried/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6497 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/curried/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      499 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/debug.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3995 2024-03-25 20:53:18.000000 eth-utils-4.1.0/eth_utils/decorators.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      199 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      110 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2100 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/functional.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1828 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/hexadecimal.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4148 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/humanize.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5155 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/logging.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      842 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/module_loading.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2244 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/network.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1190 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/numeric.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/py.typed
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2617 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/toolz.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1074 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/types.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/typing/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      325 2023-10-02 20:24:48.000000 eth-utils-4.1.0/eth_utils/typing/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      190 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/typing/misc.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1757 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/units.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/eth_utils.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5193 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2619 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      502 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       10 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3419 2024-03-25 20:53:18.000000 eth-utils-4.1.0/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-01 19:54:24.939384 eth-utils-4.1.0/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2174 2024-04-01 19:54:03.000000 eth-utils-4.1.0/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.927384 eth-utils-4.1.0/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/abi-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5031 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/abi-utils/test_abi_utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/address-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10843 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/address-utils/test_address_utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/applicator-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6721 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/applicator-utils/test_applicators.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/conversion-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4567 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/conversion-utils/test_conversions.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/currency-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4393 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/currency-utils/test_currency_tools.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      193 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/currency-utils/test_denoms_obj.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/curried-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3223 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/curried-utils/test_curried.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/decorator-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      666 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/decorator-utils/test_combomethod.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      690 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/decorator-utils/test_replace_exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1531 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/decorator-utils/test_validate_conversion_arguments.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/encoding-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1083 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/encoding-utils/test_big_endian_integer.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/functional-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1475 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/functional-utils/test_return_value_decorators.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2569 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/functional-utils/test_type_inference.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/hexadecimal-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1076 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_0x_prefix_addition_and_removal.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      487 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_0x_prefixed.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      972 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hex.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      954 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hexstr.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/humanize-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      374 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_bytes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      230 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_hash.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      714 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_integer_sequence.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1202 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_ipfs_uri.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1416 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_seconds.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1608 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_wei.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/logging-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2919 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_DEBUG2_logging.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      630 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_compat_with_abc_ABC.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2472 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_get_logger.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2760 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_has_logger_metaclass.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/module-loading-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      266 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/module-loading-utils/test_import_string.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/network-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2053 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/network-utils/test_network_utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/numeric-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      369 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/numeric-utils/test_clamp.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       91 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/test_import_and_version.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/type-checks/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2216 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_curried_utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1927 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_functional_utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1352 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_has_logger.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/types-utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3014 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/types-utils/test_types_utils.py
```

### Comparing `eth-utils-4.0.0/LICENSE` & `eth-utils-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/PKG-INFO` & `eth-utils-4.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: eth-utils
-Version: 4.0.0
+Version: 4.1.0
 Summary: eth-utils: Common utility functions for python code that interacts with Ethereum
 Home-page: https://github.com/ethereum/eth-utils
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Intended Audience :: Developers
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
-Requires-Dist: cached-property<2,>=1.5.2; python_version < "3.8"
 Requires-Dist: eth-hash>=0.3.1
 Requires-Dist: eth-typing>=3.0.0
 Requires-Dist: toolz>0.8.2; implementation_name == "pypy"
 Requires-Dist: cytoolz>=0.10.1; implementation_name == "cpython"
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
```

### Comparing `eth-utils-4.0.0/README.md` & `eth-utils-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/__init__.py` & `eth-utils-4.1.0/eth_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/__json/eth_networks.json` & `eth-utils-4.1.0/eth_utils/__json/eth_networks.json`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/abi.py` & `eth-utils-4.1.0/eth_utils/abi.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/address.py` & `eth-utils-4.1.0/eth_utils/address.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/applicators.py` & `eth-utils-4.1.0/eth_utils/applicators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/conversions.py` & `eth-utils-4.1.0/eth_utils/conversions.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/currency.py` & `eth-utils-4.1.0/eth_utils/currency.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/curried/__init__.py` & `eth-utils-4.1.0/eth_utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/decorators.py` & `eth-utils-4.1.0/eth_utils/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         )
 
 
 def _validate_supported_kwarg(kwargs: Any) -> None:
     if next(iter(kwargs)) not in ["primitive", "hexstr", "text"]:
         raise TypeError(
             "Kwarg must be 'primitive', 'hexstr', or 'text'. "
-            f"Instead, kwarg was: {repr((next(iter(kwargs))))}"
+            f"Instead, kwarg was: {repr(next(iter(kwargs)))}"
         )
 
 
 def validate_conversion_arguments(to_wrap: Callable[..., T]) -> Callable[..., T]:
     """
     Validates arguments for conversion functions.
     - Only a single argument is present
```

### Comparing `eth-utils-4.0.0/eth_utils/functional.py` & `eth-utils-4.1.0/eth_utils/functional.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/hexadecimal.py` & `eth-utils-4.1.0/eth_utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/humanize.py` & `eth-utils-4.1.0/eth_utils/humanize.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/logging.py` & `eth-utils-4.1.0/eth_utils/logging.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/module_loading.py` & `eth-utils-4.1.0/eth_utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/network.py` & `eth-utils-4.1.0/eth_utils/network.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/numeric.py` & `eth-utils-4.1.0/eth_utils/numeric.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/toolz.py` & `eth-utils-4.1.0/eth_utils/toolz.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/types.py` & `eth-utils-4.1.0/eth_utils/types.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils/units.py` & `eth-utils-4.1.0/eth_utils/units.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/eth_utils.egg-info/PKG-INFO` & `eth-utils-4.1.0/eth_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: eth-utils
-Version: 4.0.0
+Version: 4.1.0
 Summary: eth-utils: Common utility functions for python code that interacts with Ethereum
 Home-page: https://github.com/ethereum/eth-utils
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Intended Audience :: Developers
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
-Requires-Dist: cached-property<2,>=1.5.2; python_version < "3.8"
 Requires-Dist: eth-hash>=0.3.1
 Requires-Dist: eth-typing>=3.0.0
 Requires-Dist: toolz>0.8.2; implementation_name == "pypy"
 Requires-Dist: cytoolz>=0.10.1; implementation_name == "cpython"
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
```

### Comparing `eth-utils-4.0.0/eth_utils.egg-info/SOURCES.txt` & `eth-utils-4.1.0/eth_utils.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,43 +32,42 @@
 eth_utils.egg-info/not-zip-safe
 eth_utils.egg-info/requires.txt
 eth_utils.egg-info/top_level.txt
 eth_utils/__json/eth_networks.json
 eth_utils/curried/__init__.py
 eth_utils/typing/__init__.py
 eth_utils/typing/misc.py
-tests/conftest.py
-tests/abi-utils/test_abi_utils.py
-tests/address-utils/test_address_utils.py
-tests/applicator-utils/test_applicators.py
-tests/conversion-utils/test_conversions.py
 tests/core/test_import_and_version.py
-tests/currency-utils/test_currency_tools.py
-tests/currency-utils/test_denoms_obj.py
-tests/curried-utils/test_curried.py
-tests/decorator-utils/test_combomethod.py
-tests/decorator-utils/test_replace_exceptions.py
-tests/decorator-utils/test_validate_conversion_arguments.py
-tests/encoding-utils/test_big_endian_integer.py
-tests/functional-utils/test_return_value_decorators.py
-tests/functional-utils/test_type_inference.py
-tests/hexadecimal-utils/test_0x_prefix_addition_and_removal.py
-tests/hexadecimal-utils/test_is_0x_prefixed.py
-tests/hexadecimal-utils/test_is_hex.py
-tests/hexadecimal-utils/test_is_hexstr.py
-tests/humanize-utils/test_humanize_bytes.py
-tests/humanize-utils/test_humanize_hash.py
-tests/humanize-utils/test_humanize_integer_sequence.py
-tests/humanize-utils/test_humanize_ipfs_uri.py
-tests/humanize-utils/test_humanize_seconds.py
-tests/humanize-utils/test_humanize_wei.py
-tests/logging-utils/test_DEBUG2_logging.py
-tests/logging-utils/test_compat_with_abc_ABC.py
-tests/logging-utils/test_get_logger.py
-tests/logging-utils/test_has_logger_metaclass.py
-tests/module-loading-utils/test_import_string.py
-tests/network-utils/test_network_utils.py
-tests/numeric-utils/test_clamp.py
-tests/type-checks/mypy_typing_of_curried_utils.py
-tests/type-checks/mypy_typing_of_functional_utils.py
-tests/type-checks/mypy_typing_of_has_logger.py
-tests/types-utils/test_types_utils.py
+tests/core/abi-utils/test_abi_utils.py
+tests/core/address-utils/test_address_utils.py
+tests/core/applicator-utils/test_applicators.py
+tests/core/conversion-utils/test_conversions.py
+tests/core/currency-utils/test_currency_tools.py
+tests/core/currency-utils/test_denoms_obj.py
+tests/core/curried-utils/test_curried.py
+tests/core/decorator-utils/test_combomethod.py
+tests/core/decorator-utils/test_replace_exceptions.py
+tests/core/decorator-utils/test_validate_conversion_arguments.py
+tests/core/encoding-utils/test_big_endian_integer.py
+tests/core/functional-utils/test_return_value_decorators.py
+tests/core/functional-utils/test_type_inference.py
+tests/core/hexadecimal-utils/test_0x_prefix_addition_and_removal.py
+tests/core/hexadecimal-utils/test_is_0x_prefixed.py
+tests/core/hexadecimal-utils/test_is_hex.py
+tests/core/hexadecimal-utils/test_is_hexstr.py
+tests/core/humanize-utils/test_humanize_bytes.py
+tests/core/humanize-utils/test_humanize_hash.py
+tests/core/humanize-utils/test_humanize_integer_sequence.py
+tests/core/humanize-utils/test_humanize_ipfs_uri.py
+tests/core/humanize-utils/test_humanize_seconds.py
+tests/core/humanize-utils/test_humanize_wei.py
+tests/core/logging-utils/test_DEBUG2_logging.py
+tests/core/logging-utils/test_compat_with_abc_ABC.py
+tests/core/logging-utils/test_get_logger.py
+tests/core/logging-utils/test_has_logger_metaclass.py
+tests/core/module-loading-utils/test_import_string.py
+tests/core/network-utils/test_network_utils.py
+tests/core/numeric-utils/test_clamp.py
+tests/core/type-checks/mypy_typing_of_curried_utils.py
+tests/core/type-checks/mypy_typing_of_functional_utils.py
+tests/core/type-checks/mypy_typing_of_has_logger.py
+tests/core/types-utils/test_types_utils.py
```

### Comparing `eth-utils-4.0.0/pyproject.toml` & `eth-utils-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/setup.py` & `eth-utils-4.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,26 +36,25 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-utils",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="4.0.0",
+    version="4.1.0",
     description=(
         """eth-utils: Common utility functions for python code that interacts with Ethereum"""
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/eth-utils",
     include_package_data=True,
     install_requires=[
-        "cached-property>=1.5.2,<2;python_version<'3.8'",
         "eth-hash>=0.3.1",
         "eth-typing>=3.0.0",
         "toolz>0.8.2;implementation_name=='pypy'",
         "cytoolz>=0.10.1;implementation_name=='cpython'",
     ],
     python_requires=">=3.8, <4",
     extras_require=extras_require,
@@ -70,9 +69,10 @@
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

### Comparing `eth-utils-4.0.0/tests/abi-utils/test_abi_utils.py` & `eth-utils-4.1.0/tests/core/abi-utils/test_abi_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/address-utils/test_address_utils.py` & `eth-utils-4.1.0/tests/core/address-utils/test_address_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/applicator-utils/test_applicators.py` & `eth-utils-4.1.0/tests/core/applicator-utils/test_applicators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/conversion-utils/test_conversions.py` & `eth-utils-4.1.0/tests/core/conversion-utils/test_conversions.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/currency-utils/test_currency_tools.py` & `eth-utils-4.1.0/tests/core/currency-utils/test_currency_tools.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/curried-utils/test_curried.py` & `eth-utils-4.1.0/tests/core/curried-utils/test_curried.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/decorator-utils/test_combomethod.py` & `eth-utils-4.1.0/tests/core/decorator-utils/test_combomethod.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/decorator-utils/test_replace_exceptions.py` & `eth-utils-4.1.0/tests/core/decorator-utils/test_replace_exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/decorator-utils/test_validate_conversion_arguments.py` & `eth-utils-4.1.0/tests/core/decorator-utils/test_validate_conversion_arguments.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/encoding-utils/test_big_endian_integer.py` & `eth-utils-4.1.0/tests/core/encoding-utils/test_big_endian_integer.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/functional-utils/test_return_value_decorators.py` & `eth-utils-4.1.0/tests/core/functional-utils/test_return_value_decorators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/functional-utils/test_type_inference.py` & `eth-utils-4.1.0/tests/core/functional-utils/test_type_inference.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/hexadecimal-utils/test_0x_prefix_addition_and_removal.py` & `eth-utils-4.1.0/tests/core/hexadecimal-utils/test_0x_prefix_addition_and_removal.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/hexadecimal-utils/test_is_hex.py` & `eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hex.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/hexadecimal-utils/test_is_hexstr.py` & `eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hexstr.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/humanize-utils/test_humanize_integer_sequence.py` & `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_integer_sequence.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/humanize-utils/test_humanize_ipfs_uri.py` & `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_ipfs_uri.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/humanize-utils/test_humanize_seconds.py` & `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_seconds.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/humanize-utils/test_humanize_wei.py` & `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_wei.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/logging-utils/test_DEBUG2_logging.py` & `eth-utils-4.1.0/tests/core/logging-utils/test_DEBUG2_logging.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/logging-utils/test_compat_with_abc_ABC.py` & `eth-utils-4.1.0/tests/core/logging-utils/test_compat_with_abc_ABC.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/logging-utils/test_get_logger.py` & `eth-utils-4.1.0/tests/core/logging-utils/test_get_logger.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/logging-utils/test_has_logger_metaclass.py` & `eth-utils-4.1.0/tests/core/logging-utils/test_has_logger_metaclass.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/network-utils/test_network_utils.py` & `eth-utils-4.1.0/tests/core/network-utils/test_network_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/type-checks/mypy_typing_of_curried_utils.py` & `eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_curried_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/type-checks/mypy_typing_of_functional_utils.py` & `eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_functional_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/type-checks/mypy_typing_of_has_logger.py` & `eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_has_logger.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.0.0/tests/types-utils/test_types_utils.py` & `eth-utils-4.1.0/tests/core/types-utils/test_types_utils.py`

 * *Files identical despite different names*

