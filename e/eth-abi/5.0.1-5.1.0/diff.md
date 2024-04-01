# Comparing `tmp/eth_abi-5.0.1.tar.gz` & `tmp/eth_abi-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth_abi-5.0.1.tar", last modified: Mon Mar  4 21:54:18 2024, max compression
+gzip compressed data, was "eth_abi-5.1.0.tar", last modified: Mon Apr  1 19:25:04 2024, max compression
```

## Comparing `eth_abi-5.0.1.tar` & `eth_abi-5.1.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.007206 eth_abi-5.0.1/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1106 2023-12-09 19:29:35.000000 eth_abi-5.0.1/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2023-12-15 23:33:59.000000 eth_abi-5.0.1/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4960 2024-03-04 21:54:18.007206 eth_abi-5.0.1/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2627 2023-12-15 23:33:59.000000 eth_abi-5.0.1/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:17.999206 eth_abi-5.0.1/eth_abi/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      191 2023-12-15 23:33:59.000000 eth_abi-5.0.1/eth_abi/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      282 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi/abi.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4780 2024-02-15 19:48:41.000000 eth_abi-5.0.1/eth_abi/base.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5103 2024-02-15 19:48:41.000000 eth_abi-5.0.1/eth_abi/codec.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       51 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi/constants.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    20567 2024-03-04 21:51:03.000000 eth_abi-5.0.1/eth_abi/decoding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19800 2024-02-15 19:48:41.000000 eth_abi-5.0.1/eth_abi/encoding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2938 2024-03-04 21:51:03.000000 eth_abi-5.0.1/eth_abi/exceptions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12306 2024-03-01 21:08:53.000000 eth_abi-5.0.1/eth_abi/grammar.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      245 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi/packed.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-02-15 19:48:41.000000 eth_abi-5.0.1/eth_abi/py.typed
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19692 2024-03-01 21:08:53.000000 eth_abi-5.0.1/eth_abi/registry.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:17.999206 eth_abi-5.0.1/eth_abi/tools/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       51 2023-12-15 23:33:59.000000 eth_abi-5.0.1/eth_abi/tools/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5862 2023-12-15 23:33:59.000000 eth_abi-5.0.1/eth_abi/tools/_strategies.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:17.999206 eth_abi-5.0.1/eth_abi/utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi/utils/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2097 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi/utils/numeric.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      533 2023-12-15 23:33:59.000000 eth_abi-5.0.1/eth_abi/utils/padding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      436 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi/utils/string.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      540 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi/utils/validation.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/eth_abi.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4960 2024-03-04 21:54:17.000000 eth_abi-5.0.1/eth_abi.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1711 2024-03-04 21:54:17.000000 eth_abi-5.0.1/eth_abi.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-03-04 21:54:17.000000 eth_abi-5.0.1/eth_abi.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-12-09 19:29:36.000000 eth_abi-5.0.1/eth_abi.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      574 2024-03-04 21:54:17.000000 eth_abi-5.0.1/eth_abi.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        8 2024-03-04 21:54:17.000000 eth_abi-5.0.1/eth_abi.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3556 2024-02-15 19:48:41.000000 eth_abi-5.0.1/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-03-04 21:54:18.007206 eth_abi-5.0.1/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2263 2024-03-04 21:54:04.000000 eth_abi-5.0.1/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/__init__.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/abi/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/abi/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10836 2024-03-04 21:51:03.000000 eth_abi-5.0.1/tests/abi/test_decode.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4086 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/abi/test_encode.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1076 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/abi/test_is_encodable.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      407 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/abi/test_is_encodable_type.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1328 2024-01-24 19:51:32.000000 eth_abi-5.0.1/tests/abi/test_reversibility_properties.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      496 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/abi/test_uint_properties.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3996 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/base.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/common/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/common/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7306 2024-02-07 22:08:45.000000 eth_abi-5.0.1/tests/common/strategies.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    17167 2024-02-07 22:08:45.000000 eth_abi-5.0.1/tests/common/unit.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       99 2024-01-09 22:08:14.000000 eth_abi-5.0.1/tests/core/test_import_and_version.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/decoding/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/decoding/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1250 2024-02-16 19:37:26.000000 eth_abi-5.0.1/tests/decoding/test_context_frames_bytes_io.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    16746 2024-02-08 18:51:54.000000 eth_abi-5.0.1/tests/decoding/test_decoder_properties.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/encoding/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/encoding/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    14005 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/encoding/test_encoder_properties.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/end_to_end/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/end_to_end/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2629 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/end_to_end/test_custom_registrations.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8646 2023-12-15 23:33:59.000000 eth_abi-5.0.1/tests/grammar.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/packed/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/packed/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      968 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/packed/test_encode_packed.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1118 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/packed/test_is_encodable_packed.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/registry/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/registry/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6283 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/registry/test_abi_registry.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4074 2024-02-06 17:48:41.000000 eth_abi-5.0.1/tests/registry/test_predicate_mapping.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4189 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/registry/test_predicates.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4433 2023-12-15 23:33:59.000000 eth_abi-5.0.1/tests/test_tools.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-03-04 21:54:18.003206 eth_abi-5.0.1/tests/utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/utils/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      964 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/utils/test_abbr.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      364 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/utils/test_ceil32.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2004 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/utils/test_scale_places.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1705 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/utils/test_validation_utils.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      390 2023-12-09 19:29:36.000000 eth_abi-5.0.1/tests/utils/test_zpad.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.438018 eth_abi-5.1.0/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1106 2024-03-25 15:37:31.000000 eth_abi-5.1.0/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-03-25 15:37:31.000000 eth_abi-5.1.0/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5012 2024-04-01 19:25:04.438018 eth_abi-5.1.0/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2627 2024-03-25 15:37:31.000000 eth_abi-5.1.0/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.430018 eth_abi-5.1.0/eth_abi/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      191 2024-03-25 15:37:32.000000 eth_abi-5.1.0/eth_abi/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      282 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/abi.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4780 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/base.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5103 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/codec.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       51 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    20567 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/decoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19800 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/encoding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2938 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12359 2024-04-01 18:13:39.000000 eth_abi-5.1.0/eth_abi/grammar.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      245 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/packed.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-03-25 15:37:32.000000 eth_abi-5.1.0/eth_abi/py.typed
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    19692 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/registry.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.430018 eth_abi-5.1.0/eth_abi/tools/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       51 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/tools/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5862 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/tools/_strategies.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.430018 eth_abi-5.1.0/eth_abi/utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/utils/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2097 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/utils/numeric.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      533 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/utils/padding.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      436 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/utils/string.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      540 2024-03-25 15:37:31.000000 eth_abi-5.1.0/eth_abi/utils/validation.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/eth_abi.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5012 2024-04-01 19:25:03.000000 eth_abi-5.1.0/eth_abi.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1923 2024-04-01 19:25:04.000000 eth_abi-5.1.0/eth_abi.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-01 19:25:03.000000 eth_abi-5.1.0/eth_abi.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-03-25 15:37:32.000000 eth_abi-5.1.0/eth_abi.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      575 2024-04-01 19:25:03.000000 eth_abi-5.1.0/eth_abi.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        8 2024-04-01 19:25:03.000000 eth_abi-5.1.0/eth_abi.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3590 2024-04-01 18:13:39.000000 eth_abi-5.1.0/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-01 19:25:04.438018 eth_abi-5.1.0/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2314 2024-04-01 19:24:30.000000 eth_abi-5.1.0/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.430018 eth_abi-5.1.0/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/abi_tests/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/abi_tests/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10843 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/abi_tests/test_decode.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4093 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/abi_tests/test_encode.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1087 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/abi_tests/test_is_encodable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      412 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/abi_tests/test_is_encodable_type.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1333 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/abi_tests/test_reversibility_properties.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      501 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/abi_tests/test_uint_properties.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3996 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/base.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/common/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/common/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7306 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/common/strategies.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    17167 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/common/unit.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/decoding/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/decoding/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1250 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/decoding/test_context_frames_bytes_io.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    16746 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/decoding/test_decoder_properties.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/encoding/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/encoding/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    14005 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/encoding/test_encoder_properties.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/end_to_end/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/end_to_end/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2629 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/end_to_end/test_custom_registrations.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     8656 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/grammar.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/packed/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/packed/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      973 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/packed/test_encode_packed.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1129 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/packed/test_is_encodable_packed.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/registry/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/registry/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6282 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/registry/test_abi_registry.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4073 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/registry/test_predicate_mapping.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4194 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/registry/test_predicates.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       99 2024-03-25 15:37:31.000000 eth_abi-5.1.0/tests/core/test_import_and_version.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4443 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/test_tools.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:25:04.434018 eth_abi-5.1.0/tests/core/utils/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/utils/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      964 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/utils/test_abbr.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      364 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/utils/test_ceil32.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2004 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/utils/test_scale_places.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1705 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/utils/test_validation_utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      390 2024-04-01 18:13:39.000000 eth_abi-5.1.0/tests/core/utils/test_zpad.py
```

### Comparing `eth_abi-5.0.1/LICENSE` & `eth_abi-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/PKG-INFO` & `eth_abi-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth_abi
-Version: 5.0.1
+Version: 5.1.0
 Summary: eth_abi: Python utilities for working with Ethereum ABI definitions, especially encoding and decoding
 Home-page: https://github.com/ethereum/eth-abi
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,20 +12,21 @@
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
 Requires-Dist: eth-utils>=2.0.0
 Requires-Dist: eth-typing>=3.0.0
-Requires-Dist: parsimonious<0.10.0,>=0.9.0
+Requires-Dist: parsimonious<0.11.0,>=0.10.0
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

### Comparing `eth_abi-5.0.1/README.md` & `eth_abi-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/base.py` & `eth_abi-5.1.0/eth_abi/base.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/codec.py` & `eth_abi-5.1.0/eth_abi/codec.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/decoding.py` & `eth_abi-5.1.0/eth_abi/decoding.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/encoding.py` & `eth_abi-5.1.0/eth_abi/encoding.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/exceptions.py` & `eth_abi-5.1.0/eth_abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/grammar.py` & `eth_abi-5.1.0/eth_abi/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,19 +89,20 @@
     def visit_alphas(self, node, visited_children):
         return node.text
 
     def visit_digits(self, node, visited_children):
         return int(node.text)
 
     def generic_visit(self, node, visited_children):
-        if isinstance(node.expr, expressions.OneOf):
+        expr = node.expr
+        if isinstance(expr, expressions.OneOf):
             # Unwrap value chosen from alternatives
             return visited_children[0]
 
-        if isinstance(node.expr, expressions.Optional):
+        if isinstance(expr, expressions.Quantifier) and expr.min == 0 and expr.max == 1:
             # Unwrap optional value or return `None`
             if len(visited_children) != 0:
                 return visited_children[0]
 
             return None
 
         return tuple(visited_children)
```

### Comparing `eth_abi-5.0.1/eth_abi/registry.py` & `eth_abi-5.1.0/eth_abi/registry.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/tools/_strategies.py` & `eth_abi-5.1.0/eth_abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/utils/numeric.py` & `eth_abi-5.1.0/eth_abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/utils/padding.py` & `eth_abi-5.1.0/eth_abi/utils/padding.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi/utils/validation.py` & `eth_abi-5.1.0/eth_abi/utils/validation.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/eth_abi.egg-info/PKG-INFO` & `eth_abi-5.1.0/eth_abi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth_abi
-Version: 5.0.1
+Version: 5.1.0
 Summary: eth_abi: Python utilities for working with Ethereum ABI definitions, especially encoding and decoding
 Home-page: https://github.com/ethereum/eth-abi
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,20 +12,21 @@
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
 Requires-Dist: eth-utils>=2.0.0
 Requires-Dist: eth-typing>=3.0.0
-Requires-Dist: parsimonious<0.10.0,>=0.9.0
+Requires-Dist: parsimonious<0.11.0,>=0.10.0
 Provides-Extra: dev
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

### Comparing `eth_abi-5.0.1/eth_abi.egg-info/SOURCES.txt` & `eth_abi-5.1.0/eth_abi.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -24,42 +24,42 @@
 eth_abi/tools/__init__.py
 eth_abi/tools/_strategies.py
 eth_abi/utils/__init__.py
 eth_abi/utils/numeric.py
 eth_abi/utils/padding.py
 eth_abi/utils/string.py
 eth_abi/utils/validation.py
-tests/__init__.py
-tests/base.py
-tests/grammar.py
-tests/test_tools.py
-tests/abi/__init__.py
-tests/abi/test_decode.py
-tests/abi/test_encode.py
-tests/abi/test_is_encodable.py
-tests/abi/test_is_encodable_type.py
-tests/abi/test_reversibility_properties.py
-tests/abi/test_uint_properties.py
-tests/common/__init__.py
-tests/common/strategies.py
-tests/common/unit.py
+tests/core/__init__.py
+tests/core/base.py
+tests/core/grammar.py
 tests/core/test_import_and_version.py
-tests/decoding/__init__.py
-tests/decoding/test_context_frames_bytes_io.py
-tests/decoding/test_decoder_properties.py
-tests/encoding/__init__.py
-tests/encoding/test_encoder_properties.py
-tests/end_to_end/__init__.py
-tests/end_to_end/test_custom_registrations.py
-tests/packed/__init__.py
-tests/packed/test_encode_packed.py
-tests/packed/test_is_encodable_packed.py
-tests/registry/__init__.py
-tests/registry/test_abi_registry.py
-tests/registry/test_predicate_mapping.py
-tests/registry/test_predicates.py
-tests/utils/__init__.py
-tests/utils/test_abbr.py
-tests/utils/test_ceil32.py
-tests/utils/test_scale_places.py
-tests/utils/test_validation_utils.py
-tests/utils/test_zpad.py
+tests/core/test_tools.py
+tests/core/abi_tests/__init__.py
+tests/core/abi_tests/test_decode.py
+tests/core/abi_tests/test_encode.py
+tests/core/abi_tests/test_is_encodable.py
+tests/core/abi_tests/test_is_encodable_type.py
+tests/core/abi_tests/test_reversibility_properties.py
+tests/core/abi_tests/test_uint_properties.py
+tests/core/common/__init__.py
+tests/core/common/strategies.py
+tests/core/common/unit.py
+tests/core/decoding/__init__.py
+tests/core/decoding/test_context_frames_bytes_io.py
+tests/core/decoding/test_decoder_properties.py
+tests/core/encoding/__init__.py
+tests/core/encoding/test_encoder_properties.py
+tests/core/end_to_end/__init__.py
+tests/core/end_to_end/test_custom_registrations.py
+tests/core/packed/__init__.py
+tests/core/packed/test_encode_packed.py
+tests/core/packed/test_is_encodable_packed.py
+tests/core/registry/__init__.py
+tests/core/registry/test_abi_registry.py
+tests/core/registry/test_predicate_mapping.py
+tests/core/registry/test_predicates.py
+tests/core/utils/__init__.py
+tests/core/utils/test_abbr.py
+tests/core/utils/test_ceil32.py
+tests/core/utils/test_scale_places.py
+tests/core/utils/test_validation_utils.py
+tests/core/utils/test_zpad.py
```

### Comparing `eth_abi-5.0.1/eth_abi.egg-info/requires.txt` & `eth_abi-5.1.0/eth_abi.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 eth-utils>=2.0.0
 eth-typing>=3.0.0
-parsimonious<0.10.0,>=0.9.0
+parsimonious<0.11.0,>=0.10.0
 
 [dev]
 build>=0.9.0
 bumpversion>=0.5.3
 ipython
 pre-commit>=3.4.0
 tox>=4.0.0
```

### Comparing `eth_abi-5.0.1/pyproject.toml` & `eth_abi-5.1.0/pyproject.toml`

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
 known_first_party = "eth_abi"
+known_third_party = "hypothesis"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
 check_untyped_defs = true
-disallow_incomplete_defs = true
-disallow_untyped_defs = false
 disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
-disallow_subclassing_any = true
+disallow_untyped_defs = false
 ignore_missing_imports = true
-strict_optional = true
 strict_equality = true
+strict_optional = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 disable_error_code = ["arg-type", "call-arg", "call-overload", "assignment", "operator", "var-annotated", "attr-defined", "has-type", "union-attr"]
 
 
@@ -60,26 +62,26 @@
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
 # Read https://github.com/ethereum/eth-abi/blob/main/newsfragments/README.md for instructions
-package = "eth_abi"
-filename = "docs/release_notes.rst"
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "eth-abi v{version} ({project_date})"
+filename = "docs/release_notes.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/eth-abi/issues/{issue}>`__"
+package = "eth_abi"
+title_format = "eth-abi v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `eth_abi-5.0.1/setup.py` & `eth_abi-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,26 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth_abi",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="5.0.1",
+    version="5.1.0",
     description="""eth_abi: Python utilities for working with Ethereum ABI definitions, especially encoding and decoding""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/eth-abi",
     include_package_data=True,
     install_requires=[
         "eth-utils>=2.0.0",
         "eth-typing>=3.0.0",
-        "parsimonious>=0.9.0,<0.10.0",
+        "parsimonious>=0.10.0,<0.11.0",
     ],
     python_requires=">=3.8, <4",
     extras_require=extras_require,
     py_modules=["eth_abi"],
     license="MIT",
     zip_safe=False,
     keywords="ethereum",
@@ -73,9 +73,10 @@
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

### Comparing `eth_abi-5.0.1/tests/abi/test_decode.py` & `eth_abi-5.1.0/tests/core/abi_tests/test_decode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import re
-
 import pytest
+import re
 
 from eth_abi.abi import (
     decode,
 )
 from eth_abi.exceptions import (
     InsufficientDataBytes,
     InvalidPointer,
 )
 from eth_abi.grammar import (
     parse,
 )
-
-from ..common.unit import (
+from tests.core.common.unit import (
     CORRECT_DYNAMIC_ENCODINGS,
     CORRECT_STATIC_ENCODINGS,
     CORRECT_TUPLE_ENCODINGS,
     words,
 )
```

### Comparing `eth_abi-5.0.1/tests/abi/test_encode.py` & `eth_abi-5.1.0/tests/core/abi_tests/test_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import re
-
 import pytest
+import re
 
 from eth_abi import (
     encode,
 )
 from eth_abi.grammar import (
     parse,
 )
-
-from ..common.unit import (
+from tests.core.common.unit import (
     CORRECT_DYNAMIC_ENCODINGS,
     CORRECT_STATIC_ENCODINGS,
     CORRECT_TUPLE_ENCODINGS,
     words,
 )
```

### Comparing `eth_abi-5.0.1/tests/abi/test_is_encodable.py` & `eth_abi-5.1.0/tests/core/abi_tests/test_is_encodable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import pytest
+
 from hypothesis import (
     given,
     settings,
 )
-import pytest
 
 from eth_abi import (
     is_encodable,
 )
-from tests.common.strategies import (
+from tests.core.common.strategies import (
     single_strs_values,
     tuple_strs_values,
 )
-from tests.common.unit import (
+from tests.core.common.unit import (
     CORRECT_ENCODINGS,
     NOT_ENCODABLE,
 )
 
 
 @pytest.mark.parametrize(
     "type_str,python_value,_1,_2",
```

### Comparing `eth_abi-5.0.1/tests/abi/test_reversibility_properties.py` & `eth_abi-5.1.0/tests/core/abi_tests/test_reversibility_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     settings,
 )
 
 from eth_abi import (
     decode,
     encode,
 )
-from tests.common.strategies import (
+from tests.core.common.strategies import (
     multi_strs_values,
     single_strs_values,
     tuple_strs_values,
 )
 
 
 @settings(deadline=None)
```

### Comparing `eth_abi-5.0.1/tests/base.py` & `eth_abi-5.1.0/tests/core/base.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/tests/common/strategies.py` & `eth_abi-5.1.0/tests/core/common/strategies.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/tests/common/unit.py` & `eth_abi-5.1.0/tests/core/common/unit.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/tests/decoding/test_context_frames_bytes_io.py` & `eth_abi-5.1.0/tests/core/decoding/test_context_frames_bytes_io.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/tests/decoding/test_decoder_properties.py` & `eth_abi-5.1.0/tests/core/decoding/test_decoder_properties.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pytest
 import sys
 
 from eth_utils import (
     big_endian_to_int,
     decode_hex,
     int_to_big_endian,
     to_normalized_address,
@@ -11,15 +12,14 @@
 )
 from hypothesis import (
     example,
     given,
     settings,
     strategies as st,
 )
-import pytest
 
 from eth_abi import (
     decode,
     encode,
 )
 from eth_abi.constants import (
     TT256M1,
```

### Comparing `eth_abi-5.0.1/tests/encoding/test_encoder_properties.py` & `eth_abi-5.1.0/tests/core/encoding/test_encoder_properties.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import codecs
 import decimal
+import pytest
 
 from eth_utils import (
     decode_hex,
     int_to_big_endian,
     is_address,
     is_boolean,
     is_bytes,
@@ -16,15 +17,14 @@
 )
 from hypothesis import (
     example,
     given,
     settings,
     strategies as st,
 )
-import pytest
 
 from eth_abi.encoding import (
     AddressEncoder,
     BooleanEncoder,
     BytesEncoder,
     ByteStringEncoder,
     SignedFixedEncoder,
```

### Comparing `eth_abi-5.0.1/tests/end_to_end/test_custom_registrations.py` & `eth_abi-5.1.0/tests/core/end_to_end/test_custom_registrations.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/tests/grammar.py` & `eth_abi-5.1.0/tests/core/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+import pytest
+
 from hypothesis import (
     example,
     given,
     strategies as st,
 )
-import pytest
 
 from eth_abi.exceptions import (
     ABITypeError,
     ParseError,
 )
 from eth_abi.grammar import (
     TYPE_ALIASES,
     BasicType,
     TupleType,
     normalize,
     parse,
 )
-
-from .common.strategies import (
+from tests.core.common.strategies import (
     malformed_type_strs,
     type_strs,
 )
 
 
 @pytest.mark.parametrize(
     "type_str, expected_type",
```

### Comparing `eth_abi-5.0.1/tests/packed/test_encode_packed.py` & `eth_abi-5.1.0/tests/core/packed/test_encode_packed.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from eth_abi.grammar import (
     parse,
 )
 from eth_abi.packed import (
     encode_packed,
 )
-from tests.common.unit import (
+from tests.core.common.unit import (
     CORRECT_ENCODINGS,
     CORRECT_TUPLE_ENCODINGS,
 )
 
 
 @pytest.mark.parametrize(
     "single_abi_type,python_value,_,packed_encoding",
```

### Comparing `eth_abi-5.0.1/tests/packed/test_is_encodable_packed.py` & `eth_abi-5.1.0/tests/core/packed/test_is_encodable_packed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import pytest
+
 from hypothesis import (
     given,
     settings,
 )
-import pytest
 
 from eth_abi.packed import (
     is_encodable_packed,
 )
-from tests.common.strategies import (
+from tests.core.common.strategies import (
     single_strs_values,
     tuple_strs_values,
 )
-from tests.common.unit import (
+from tests.core.common.unit import (
     CORRECT_ENCODINGS,
     NOT_ENCODABLE,
 )
 
 
 @pytest.mark.parametrize(
     "type_str,python_value,_1,_2",
```

### Comparing `eth_abi-5.0.1/tests/registry/test_abi_registry.py` & `eth_abi-5.1.0/tests/core/registry/test_abi_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
 import itertools
-
 import pytest
 
 from eth_abi import (
     decoding,
     encoding,
     exceptions,
 )
```

### Comparing `eth_abi-5.0.1/tests/registry/test_predicate_mapping.py` & `eth_abi-5.1.0/tests/core/registry/test_predicate_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 import functools
 import itertools
 import operator
-
 import pytest
 
 from eth_abi.registry import (
     Equals,
     PredicateMapping,
 )
```

### Comparing `eth_abi-5.0.1/tests/registry/test_predicates.py` & `eth_abi-5.1.0/tests/core/registry/test_predicates.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from eth_abi.registry import (
     BaseEquals,
     Equals,
     has_arrlist,
     is_base_tuple,
 )
-from tests.common.strategies import (
+from tests.core.common.strategies import (
     malformed_type_strs,
     type_strs,
 )
 
 
 @given(st.text())
 def test_equals_has_expected_behavior(s):
```

### Comparing `eth_abi-5.0.1/tests/test_tools.py` & `eth_abi-5.1.0/tests/core/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+import pytest
+
 from hypothesis import (
     example,
     given,
     settings,
     strategies as st,
 )
-import pytest
 
 from eth_abi.exceptions import (
     NoEntriesFound,
     ParseError,
 )
 from eth_abi.tools import (
     get_abi_strategy,
 )
-
-from .common.strategies import (
+from tests.core.common.strategies import (
     malformed_type_strs,
     type_strs,
 )
 
 
 @given(type_strs)
 @settings(deadline=None)
```

### Comparing `eth_abi-5.0.1/tests/utils/test_abbr.py` & `eth_abi-5.1.0/tests/core/utils/test_abbr.py`

 * *Files identical despite different names*

### Comparing `eth_abi-5.0.1/tests/utils/test_scale_places.py` & `eth_abi-5.1.0/tests/core/utils/test_scale_places.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import decimal
 import itertools
+import pytest
 from typing import (
     Iterable,
     Iterator,
     TypeVar,
 )
 
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 from eth_abi.utils.numeric import (
     ABI_DECIMAL_PREC,
     scale_places,
 )
 
 T = TypeVar("T")
```

### Comparing `eth_abi-5.0.1/tests/utils/test_validation_utils.py` & `eth_abi-5.1.0/tests/core/utils/test_validation_utils.py`

 * *Files identical despite different names*

