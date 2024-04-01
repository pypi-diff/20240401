# Comparing `tmp/ssz-0.4.0.tar.gz` & `tmp/ssz-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssz-0.4.0.tar", last modified: Thu Dec  7 21:47:44 2023, max compression
+gzip compressed data, was "ssz-0.5.0.tar", last modified: Mon Apr  1 19:19:18 2024, max compression
```

## Comparing `ssz-0.4.0.tar` & `ssz-0.5.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.773617 ssz-0.4.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2023-04-19 19:56:01.000000 ssz-0.4.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2023-12-07 21:01:11.000000 ssz-0.4.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4512 2023-12-07 21:47:44.773617 ssz-0.4.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2530 2023-12-07 21:01:11.000000 ssz-0.4.0/README.md
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3505 2023-12-07 21:01:11.000000 ssz-0.4.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2023-12-07 21:47:44.773617 ssz-0.4.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2268 2023-12-07 21:47:15.000000 ssz-0.4.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.761617 ssz-0.4.0/ssz/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      729 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3556 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/abc.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.765617 ssz-0.4.0/ssz/cache/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       37 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/cache/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1394 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/cache/cache.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1244 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/cache/utils.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1062 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/codec.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      595 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/constants.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      311 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/exceptions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      383 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/hash.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    13252 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/hash_tree.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12159 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/hashable_container.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      776 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/hashable_list.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    15009 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/hashable_structure.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      934 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/hashable_vector.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-19 18:16:07.000000 ssz-0.4.0/ssz/py.typed
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/ssz/sedes/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1822 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1996 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/base.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6125 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/basic.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3709 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/bitlist.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2587 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/bitvector.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1161 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/boolean.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      982 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/byte.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1977 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/byte_list.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2101 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/byte_vector.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6736 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/container.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6324 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/list.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    13735 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/serializable.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1975 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/signed_serializable.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1544 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/uint.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5504 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/sedes/vector.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/ssz/tools/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      134 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/tools/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      721 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/tools/codec.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3876 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/tools/dump.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4396 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/tools/parse.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      336 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/tree_hash.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      353 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/typing.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6789 2023-12-07 21:01:11.000000 ssz-0.4.0/ssz/utils.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/ssz.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4512 2023-12-07 21:47:44.000000 ssz-0.4.0/ssz.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1914 2023-12-07 21:47:44.000000 ssz-0.4.0/ssz.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-12-07 21:47:44.000000 ssz-0.4.0/ssz.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-04-19 18:18:12.000000 ssz-0.4.0/ssz.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      424 2023-12-07 21:47:44.000000 ssz-0.4.0/ssz.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        4 2023-12-07 21:47:44.000000 ssz-0.4.0/ssz.egg-info/top_level.txt
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-19 18:16:07.000000 ssz-0.4.0/tests/__init__.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       48 2023-04-19 19:56:01.000000 ssz-0.4.0/tests/core/test_import.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/hashable/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-19 18:16:07.000000 ssz-0.4.0/tests/hashable/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1883 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/hashable/chunk_strategies.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11528 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/hashable/hashable_strategies.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5454 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/hashable/test_chunk_updates.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3958 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/hashable/test_hash_tree.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12783 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/hashable/test_hashable_structures.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/misc/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-19 18:16:07.000000 ssz-0.4.0/tests/misc/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      952 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/misc/test_cache.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3099 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/misc/test_serializable.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3587 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/misc/test_serializable_inheritance.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1769 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/misc/test_signed_serializable.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2621 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/misc/test_utils.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/sedes/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2326 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/sedes/test_basic_sedes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2449 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/sedes/test_bitlist_serializer.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      187 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/sedes/test_bitvector_instantiation.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1903 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/sedes/test_bitvector_serializer.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6749 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/sedes/test_composite_sedes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1215 2023-04-19 18:16:07.000000 ssz-0.4.0/tests/sedes/test_fixed_size_sedes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2353 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/sedes/test_sedes_aliases.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/tools/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1327 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/tools/test_parsing_and_dumping.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/tree_hash/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-19 18:16:07.000000 ssz-0.4.0/tests/tree_hash/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1251 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/tree_hash/test_aliases_tree_hash.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      882 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/tree_hash/test_basic_sedes_trie_hash.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5808 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/tree_hash/test_composite_tree_hash.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-07 21:47:44.769617 ssz-0.4.0/tests/yaml_tests/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1612 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/yaml_tests/test_yaml.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3762 2023-12-07 21:01:11.000000 ssz-0.4.0/tests/yaml_tests/yaml_test_execution.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.967807 ssz-0.5.0/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2024-03-25 16:35:16.000000 ssz-0.5.0/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-03-25 16:35:16.000000 ssz-0.5.0/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4563 2024-04-01 19:19:18.967807 ssz-0.5.0/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2530 2024-03-25 16:35:16.000000 ssz-0.5.0/README.md
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3503 2024-04-01 18:08:51.000000 ssz-0.5.0/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-01 19:19:18.967807 ssz-0.5.0/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2318 2024-04-01 19:18:57.000000 ssz-0.5.0/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.959807 ssz-0.5.0/ssz/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      729 2024-03-25 16:35:18.000000 ssz-0.5.0/ssz/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3556 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/abc.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.959807 ssz-0.5.0/ssz/cache/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       37 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/cache/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1394 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/cache/cache.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1244 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/cache/utils.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1062 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/codec.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      595 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      311 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/exceptions.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      383 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/hash.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    13252 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/hash_tree.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12159 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/hashable_container.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      776 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/hashable_list.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    15009 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/hashable_structure.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      934 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/hashable_vector.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-03-25 16:35:18.000000 ssz-0.5.0/ssz/py.typed
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/ssz/sedes/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1822 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1996 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/base.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6125 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/basic.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3709 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/bitlist.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2587 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/bitvector.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1161 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/boolean.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      982 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/byte.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1977 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/byte_list.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2101 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/byte_vector.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6736 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/container.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6324 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/list.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    13733 2024-04-01 18:08:51.000000 ssz-0.5.0/ssz/sedes/serializable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1975 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/signed_serializable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1544 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/uint.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5504 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/sedes/vector.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/ssz/tools/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      134 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/tools/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      721 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/tools/codec.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3876 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/tools/dump.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4396 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/tools/parse.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      336 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/tree_hash.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      353 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/typing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6789 2024-03-25 16:35:16.000000 ssz-0.5.0/ssz/utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.967807 ssz-0.5.0/ssz.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     4563 2024-04-01 19:19:18.000000 ssz-0.5.0/ssz.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2069 2024-04-01 19:19:18.000000 ssz-0.5.0/ssz.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-01 19:19:18.000000 ssz-0.5.0/ssz.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-03-25 16:35:18.000000 ssz-0.5.0/ssz.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      424 2024-04-01 19:19:18.000000 ssz-0.5.0/ssz.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        4 2024-04-01 19:19:18.000000 ssz-0.5.0/ssz.egg-info/top_level.txt
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/tests/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-03-25 16:38:28.000000 ssz-0.5.0/tests/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/tests/core/hashable/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/hashable/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1883 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/hashable/chunk_strategies.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11528 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/hashable/hashable_strategies.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5459 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/hashable/test_chunk_updates.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3964 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/hashable/test_hash_tree.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12788 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/hashable/test_hashable_structures.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/tests/core/misc/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/misc/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      952 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/misc/test_cache.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3099 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/misc/test_serializable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3587 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/misc/test_serializable_inheritance.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1769 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/misc/test_signed_serializable.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2622 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/misc/test_utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/tests/core/sedes/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2327 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/sedes/test_basic_sedes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2449 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/sedes/test_bitlist_serializer.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      187 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/sedes/test_bitvector_instantiation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1903 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/sedes/test_bitvector_serializer.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6749 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/sedes/test_composite_sedes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1215 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/sedes/test_fixed_size_sedes.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2354 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/sedes/test_sedes_aliases.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       91 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/test_import_and_version.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.963807 ssz-0.5.0/tests/core/tools/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1327 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/tools/test_parsing_and_dumping.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.967807 ssz-0.5.0/tests/core/tree_hash/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/tree_hash/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1252 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/tree_hash/test_aliases_tree_hash.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      883 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/tree_hash/test_basic_sedes_trie_hash.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5807 2024-04-01 18:08:51.000000 ssz-0.5.0/tests/core/tree_hash/test_composite_tree_hash.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:19:18.967807 ssz-0.5.0/tests/yaml_tests/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1612 2024-03-25 16:35:18.000000 ssz-0.5.0/tests/yaml_tests/test_yaml.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3762 2024-03-25 16:35:18.000000 ssz-0.5.0/tests/yaml_tests/yaml_test_execution.py
```

### Comparing `ssz-0.4.0/LICENSE` & `ssz-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/PKG-INFO` & `ssz-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssz
-Version: 0.4.0
+Version: 0.5.0
 Summary: ssz: Python implementation of the Simple Serialization encoding and decoding
 Home-page: https://github.com/ethereum/py-ssz
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
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
 Requires-Dist: eth-utils>=2
 Requires-Dist: lru-dict>=1.1.6
 Requires-Dist: pyrsistent<0.17,>=0.16.0
 Provides-Extra: dev
```

### Comparing `ssz-0.4.0/README.md` & `ssz-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/pyproject.toml` & `ssz-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.autoflake]
-remove_all_unused_imports = "True"
 exclude = "__init__.py"
+remove_all_unused_imports = true
 
 [tool.isort]
-combine_as_imports = "True"
+combine_as_imports = true
 extra_standard_library = "pytest"
 force_grid_wrap = 1
-force_sort_within_sections = "True"
-known_third_party = "hypothesis,pytest,eth_typing,eth_utils,lru,pyrsistent,ruamel,setuptools,yaml_test_execution"
+force_sort_within_sections = true
+honor_noqa = true
 known_first_party = "ssz"
+known_third_party = "hypothesis,eth_typing,eth_utils,lru,pyrsistent,ruamel,setuptools,yaml_test_execution"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
-check_untyped_defs = "True"
-disallow_incomplete_defs = "True"
-disallow_untyped_defs = "True"
-disallow_any_generics = "True"
-disallow_untyped_calls = "True"
-disallow_untyped_decorators = "True"
-disallow_subclassing_any = "True"
-ignore_missing_imports = "True"
-strict_optional = "True"
-strict_equality = "True"
-warn_redundant_casts = "True"
-warn_return_any = "True"
-warn_unused_configs = "True"
-warn_unused_ignores = "True"
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_decorators = true
+disallow_untyped_defs = true
+ignore_missing_imports = true
+strict_equality = true
+strict_optional = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unused_configs = true
+warn_unused_ignores = true
 
 
 [tool.pydocstyle]
 # All error codes found here:
 # http://www.pydocstyle.org/en/3.0.0/error_codes.html
 #
 # Ignored:
@@ -59,26 +61,26 @@
 # D400 - Enabling this error code seems to make it a requirement that the first
 # sentence in a docstring is not split across two lines.  It also makes it a
 # requirement that no docstring can have a multi-sentence description without a
 # summary line.  Neither one of those requirements seem appropriate.
 
 [tool.pytest.ini_options]
 addopts = "-v --showlocals --durations 10"
-xfail_strict = "True"
-log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 log_date_format = "%m-%d %H:%M:%S"
+log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
+xfail_strict = true
 
 [tool.towncrier]
 # Read https://github.com/ethereum/py-ssz/blob/main/newsfragments/README.md for instructions
-package = "ssz"
-filename = "docs/release_notes.rst"
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "py-ssz v{version} ({project_date})"
+filename = "docs/release_notes.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/py-ssz/issues/{issue}>`__"
+package = "ssz"
+title_format = "py-ssz v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `ssz-0.4.0/setup.py` & `ssz-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="ssz",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="0.4.0",
+    version="0.5.0",
     description="""ssz: Python implementation of the Simple Serialization encoding and decoding""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/py-ssz",
     include_package_data=True,
@@ -72,9 +72,10 @@
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

### Comparing `ssz-0.4.0/ssz/__init__.py` & `ssz-0.5.0/ssz/__init__.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/abc.py` & `ssz-0.5.0/ssz/abc.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/cache/cache.py` & `ssz-0.5.0/ssz/cache/cache.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/cache/utils.py` & `ssz-0.5.0/ssz/cache/utils.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/codec.py` & `ssz-0.5.0/ssz/codec.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/constants.py` & `ssz-0.5.0/ssz/constants.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/hash_tree.py` & `ssz-0.5.0/ssz/hash_tree.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/hashable_container.py` & `ssz-0.5.0/ssz/hashable_container.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/hashable_list.py` & `ssz-0.5.0/ssz/hashable_list.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/hashable_structure.py` & `ssz-0.5.0/ssz/hashable_structure.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/hashable_vector.py` & `ssz-0.5.0/ssz/hashable_vector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/__init__.py` & `ssz-0.5.0/ssz/sedes/__init__.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/base.py` & `ssz-0.5.0/ssz/sedes/base.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/basic.py` & `ssz-0.5.0/ssz/sedes/basic.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/bitlist.py` & `ssz-0.5.0/ssz/sedes/bitlist.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/bitvector.py` & `ssz-0.5.0/ssz/sedes/bitvector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/boolean.py` & `ssz-0.5.0/ssz/sedes/boolean.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/byte.py` & `ssz-0.5.0/ssz/sedes/byte.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/byte_list.py` & `ssz-0.5.0/ssz/sedes/byte_list.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/byte_vector.py` & `ssz-0.5.0/ssz/sedes/byte_vector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/container.py` & `ssz-0.5.0/ssz/sedes/container.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/list.py` & `ssz-0.5.0/ssz/sedes/list.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/serializable.py` & `ssz-0.5.0/ssz/sedes/serializable.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,11 +422,11 @@
 
 class Serializable(BaseSerializable, metaclass=MetaSerializable):
     """
     The base class for serializable objects.
     """
 
     def __str__(self) -> str:
-        return f"[{', '.join((str(v) for v in self))}]"
+        return f"[{', '.join(str(v) for v in self)}]"
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {str(self)}>"
```

### Comparing `ssz-0.4.0/ssz/sedes/signed_serializable.py` & `ssz-0.5.0/ssz/sedes/signed_serializable.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/uint.py` & `ssz-0.5.0/ssz/sedes/uint.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/sedes/vector.py` & `ssz-0.5.0/ssz/sedes/vector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/tools/codec.py` & `ssz-0.5.0/ssz/tools/codec.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/tools/dump.py` & `ssz-0.5.0/ssz/tools/dump.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/tools/parse.py` & `ssz-0.5.0/ssz/tools/parse.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz/utils.py` & `ssz-0.5.0/ssz/utils.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/ssz.egg-info/PKG-INFO` & `ssz-0.5.0/ssz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssz
-Version: 0.4.0
+Version: 0.5.0
 Summary: ssz: Python implementation of the Simple Serialization encoding and decoding
 Home-page: https://github.com/ethereum/py-ssz
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
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
 Requires-Dist: eth-utils>=2
 Requires-Dist: lru-dict>=1.1.6
 Requires-Dist: pyrsistent<0.17,>=0.16.0
 Provides-Extra: dev
```

### Comparing `ssz-0.4.0/ssz.egg-info/SOURCES.txt` & `ssz-0.5.0/ssz.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -43,34 +43,35 @@
 ssz/sedes/uint.py
 ssz/sedes/vector.py
 ssz/tools/__init__.py
 ssz/tools/codec.py
 ssz/tools/dump.py
 ssz/tools/parse.py
 tests/__init__.py
-tests/core/test_import.py
-tests/hashable/__init__.py
-tests/hashable/chunk_strategies.py
-tests/hashable/hashable_strategies.py
-tests/hashable/test_chunk_updates.py
-tests/hashable/test_hash_tree.py
-tests/hashable/test_hashable_structures.py
-tests/misc/__init__.py
-tests/misc/test_cache.py
-tests/misc/test_serializable.py
-tests/misc/test_serializable_inheritance.py
-tests/misc/test_signed_serializable.py
-tests/misc/test_utils.py
-tests/sedes/test_basic_sedes.py
-tests/sedes/test_bitlist_serializer.py
-tests/sedes/test_bitvector_instantiation.py
-tests/sedes/test_bitvector_serializer.py
-tests/sedes/test_composite_sedes.py
-tests/sedes/test_fixed_size_sedes.py
-tests/sedes/test_sedes_aliases.py
-tests/tools/test_parsing_and_dumping.py
-tests/tree_hash/__init__.py
-tests/tree_hash/test_aliases_tree_hash.py
-tests/tree_hash/test_basic_sedes_trie_hash.py
-tests/tree_hash/test_composite_tree_hash.py
+tests/core/__init__.py
+tests/core/test_import_and_version.py
+tests/core/hashable/__init__.py
+tests/core/hashable/chunk_strategies.py
+tests/core/hashable/hashable_strategies.py
+tests/core/hashable/test_chunk_updates.py
+tests/core/hashable/test_hash_tree.py
+tests/core/hashable/test_hashable_structures.py
+tests/core/misc/__init__.py
+tests/core/misc/test_cache.py
+tests/core/misc/test_serializable.py
+tests/core/misc/test_serializable_inheritance.py
+tests/core/misc/test_signed_serializable.py
+tests/core/misc/test_utils.py
+tests/core/sedes/test_basic_sedes.py
+tests/core/sedes/test_bitlist_serializer.py
+tests/core/sedes/test_bitvector_instantiation.py
+tests/core/sedes/test_bitvector_serializer.py
+tests/core/sedes/test_composite_sedes.py
+tests/core/sedes/test_fixed_size_sedes.py
+tests/core/sedes/test_sedes_aliases.py
+tests/core/tools/test_parsing_and_dumping.py
+tests/core/tree_hash/__init__.py
+tests/core/tree_hash/test_aliases_tree_hash.py
+tests/core/tree_hash/test_basic_sedes_trie_hash.py
+tests/core/tree_hash/test_composite_tree_hash.py
 tests/yaml_tests/test_yaml.py
 tests/yaml_tests/yaml_test_execution.py
```

### Comparing `ssz-0.4.0/tests/hashable/chunk_strategies.py` & `ssz-0.5.0/tests/core/hashable/chunk_strategies.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/hashable/hashable_strategies.py` & `ssz-0.5.0/tests/core/hashable/hashable_strategies.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/hashable/test_chunk_updates.py` & `ssz-0.5.0/tests/core/hashable/test_chunk_updates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ssz.hashable_structure import (
     get_appended_chunks,
     get_num_padding_elements,
     get_updated_chunks,
     update_element_in_chunk,
     update_elements_in_chunk,
 )
-from tests.hashable.chunk_strategies import (
+from tests.core.hashable.chunk_strategies import (
     chunk_st,
     chunk_updates_st,
     element_size_st,
     element_st,
     elements_st,
     in_chunk_index_and_element_st,
 )
```

### Comparing `ssz-0.4.0/tests/hashable/test_hash_tree.py` & `ssz-0.5.0/tests/core/hashable/test_hash_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import pytest
+
 from hypothesis import (
     assume,
     given,
     strategies as st,
 )
-import pytest
 
 from ssz.constants import (
     ZERO_HASHES,
 )
 from ssz.hash_tree import (
     HashTree,
 )
 from ssz.utils import (
     merkleize,
 )
-from tests.hashable.chunk_strategies import (
+from tests.core.hashable.chunk_strategies import (
     chunk_st,
     chunks_and_chunk_count_st,
     hash_tree_st,
 )
 
 
 @given(chunks_and_chunk_count_st())
```

### Comparing `ssz-0.4.0/tests/hashable/test_hashable_structures.py` & `ssz-0.5.0/tests/core/hashable/test_hashable_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import ssz
 from ssz.hashable_container import (
     SignedHashableContainer,
 )
 from ssz.sedes import (
     bytes96,
 )
-from tests.hashable.hashable_strategies import (
+from tests.core.hashable.hashable_strategies import (
     composite_sedes_and_values_st,
     container_sedes_and_values_st,
     list_sedes_and_values_st,
     to_hashable_value,
     to_plain_value,
     to_serializable_value,
     transform_path_st,
```

### Comparing `ssz-0.4.0/tests/misc/test_cache.py` & `ssz-0.5.0/tests/core/misc/test_cache.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/misc/test_serializable.py` & `ssz-0.5.0/tests/core/misc/test_serializable.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/misc/test_serializable_inheritance.py` & `ssz-0.5.0/tests/core/misc/test_serializable_inheritance.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/misc/test_signed_serializable.py` & `ssz-0.5.0/tests/core/misc/test_signed_serializable.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/misc/test_utils.py` & `ssz-0.5.0/tests/core/misc/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 from ssz.constants import (
     CHUNK_SIZE,
     EMPTY_CHUNK,
     MAX_ZERO_HASHES_LAYER,
 )
 from ssz.hash import (
```

### Comparing `ssz-0.4.0/tests/sedes/test_basic_sedes.py` & `ssz-0.5.0/tests/core/sedes/test_basic_sedes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from eth_utils import (
     decode_hex,
     encode_hex,
 )
-import pytest
 
 import ssz
 from ssz.sedes import (
     Boolean,
     Byte,
     UInt,
     Vector,
```

### Comparing `ssz-0.4.0/tests/sedes/test_bitlist_serializer.py` & `ssz-0.5.0/tests/core/sedes/test_bitlist_serializer.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/sedes/test_bitvector_serializer.py` & `ssz-0.5.0/tests/core/sedes/test_bitvector_serializer.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/sedes/test_composite_sedes.py` & `ssz-0.5.0/tests/core/sedes/test_composite_sedes.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
+import pytest
 
 from eth_utils import (
     decode_hex,
     encode_hex,
 )
-import pytest
 
 import ssz
 from ssz.exceptions import (
     DeserializationError,
 )
 from ssz.hashable_list import (
     HashableList,
```

### Comparing `ssz-0.4.0/tests/sedes/test_fixed_size_sedes.py` & `ssz-0.5.0/tests/core/sedes/test_fixed_size_sedes.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/sedes/test_sedes_aliases.py` & `ssz-0.5.0/tests/core/sedes/test_sedes_aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 import ssz
 from ssz.exceptions import (
     DeserializationError,
     SerializationError,
 )
 from ssz.sedes import (
```

### Comparing `ssz-0.4.0/tests/tools/test_parsing_and_dumping.py` & `ssz-0.5.0/tests/core/tools/test_parsing_and_dumping.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/tree_hash/test_aliases_tree_hash.py` & `ssz-0.5.0/tests/core/tree_hash/test_aliases_tree_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 import ssz
 from ssz.sedes import (
     ByteList,
     ByteVector,
     List,
     Vector,
```

### Comparing `ssz-0.4.0/tests/tree_hash/test_basic_sedes_trie_hash.py` & `ssz-0.5.0/tests/core/tree_hash/test_basic_sedes_trie_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 import ssz
 from ssz.constants import (
     CHUNK_SIZE,
 )
 from ssz.sedes import (
     UInt,
```

### Comparing `ssz-0.4.0/tests/tree_hash/test_composite_tree_hash.py` & `ssz-0.5.0/tests/core/tree_hash/test_composite_tree_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import itertools
-
 import pytest
 
 import ssz
 from ssz.constants import (
     CHUNK_SIZE,
     EMPTY_CHUNK,
 )
```

### Comparing `ssz-0.4.0/tests/yaml_tests/test_yaml.py` & `ssz-0.5.0/tests/yaml_tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `ssz-0.4.0/tests/yaml_tests/yaml_test_execution.py` & `ssz-0.5.0/tests/yaml_tests/yaml_test_execution.py`

 * *Files identical despite different names*

