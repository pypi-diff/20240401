# Comparing `tmp/pydantic-kedro-0.7.0.tar.gz` & `tmp/pydantic-kedro-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.7.0.tar", last modified: Fri Mar 22 14:59:31 2024, max compression
+gzip compressed data, was "pydantic-kedro-0.8.0.tar", last modified: Mon Apr  1 20:16:55 2024, max compression
```

## Comparing `pydantic-kedro-0.7.0.tar` & `pydantic-kedro-0.8.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.494974 pydantic-kedro-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.482974 pydantic-kedro-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.482974 pydantic-kedro-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-22 14:59:31.494974 pydantic-kedro-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.482974 pydantic-kedro-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/docs/arbitrary_types.md
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/docs/standalone_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 14:59:31.494974 pydantic-kedro-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.478974 pydantic-kedro-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.486974 pydantic-kedro-0.7.0/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/_dict_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/_local_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.486974 pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.490974 pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-22 14:59:31.000000 pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-22 14:59:31.000000 pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:59:31.000000 pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:57:56.000000 pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-22 14:59:31.000000 pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-22 14:59:31.000000 pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.490974 pydantic-kedro-0.7.0/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.490974 pydantic-kedro-0.7.0/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.482974 pydantic-kedro-0.7.0/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.490974 pydantic-kedro-0.7.0/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.490974 pydantic-kedro-0.7.0/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:59:31.490974 pydantic-kedro-0.7.0/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_docs_standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_ds_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_nested_subtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_strict.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-22 14:57:45.000000 pydantic-kedro-0.7.0/src/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.797609 pydantic-kedro-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.785609 pydantic-kedro-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.785609 pydantic-kedro-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-01 20:16:55.797609 pydantic-kedro-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.785609 pydantic-kedro-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/docs/standalone_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/env-v1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:16:55.797609 pydantic-kedro-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.781609 pydantic-kedro-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.785609 pydantic-kedro-0.8.0/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/_dict_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/_local_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/_pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.789609 pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.793609 pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-01 20:16:55.000000 pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-01 20:16:55.000000 pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:16:55.000000 pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:15:11.000000 pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 20:16:55.000000 pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 20:16:55.000000 pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.793609 pydantic-kedro-0.8.0/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.793609 pydantic-kedro-0.8.0/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.781609 pydantic-kedro-0.8.0/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.793609 pydantic-kedro-0.8.0/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.793609 pydantic-kedro-0.8.0/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:16:55.793609 pydantic-kedro-0.8.0/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_docs_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_ds_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_nested_subtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_strict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-01 20:15:00.000000 pydantic-kedro-0.8.0/src/test/test_utils.py
```

### Comparing `pydantic-kedro-0.7.0/.github/dependabot.yml` & `pydantic-kedro-0.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/.github/workflows/python-publish.yml` & `pydantic-kedro-0.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/.github/workflows/python-testing.yml` & `pydantic-kedro-0.8.0/.github/workflows/python-testing.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
       fail-fast: false
       matrix:
         python-version:
           - "3.9"
           - "3.10"
         lib-pydantic:
           - "1.10.0"
+          - "2.6.4"
         deps:
           - dev,docs
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
```

### Comparing `pydantic-kedro-0.7.0/.pre-commit-config.yaml` & `pydantic-kedro-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/LICENSE` & `pydantic-kedro-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/PKG-INFO` & `pydantic-kedro-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.7.0
+Version: 0.8.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,16 +31,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic<2,>=1.10.0
-Requires-Dist: pydantic-yaml>=1.1.2
+Requires-Dist: pydantic<3,>=1.10.0
+Requires-Dist: pydantic-yaml>=1.3.0
 Requires-Dist: ruamel-yaml<0.18
 Requires-Dist: kedro<0.20,>=0.19.3
 Requires-Dist: kedro-datasets>=2.1.0
 Requires-Dist: fsspec
 Provides-Extra: dev
 Requires-Dist: setuptools>=61.0.0; extra == "dev"
 Requires-Dist: setuptools-scm[toml]>=6.2; extra == "dev"
@@ -91,14 +91,15 @@
 ## Direct Dataset Usage
 
 This example works for "pure", JSON-safe Pydantic models via
 `PydanticJsonDataset`:
 
 ```python
 from pydantic import BaseModel
+# from pydantic.v1 import BaseModel  # Pydantic V2
 from pydantic_kedro import PydanticJsonDataset
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
 
     x: int
@@ -120,15 +121,15 @@
 
 You can also use `pydantic-kedro` as a generic saving and loading engine for
 Pydantic models:
 
 ```python
 from tempfile import TemporaryDirectory
 
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 from pydantic_kedro import load_model, save_model
 
 class MyModel(BaseModel):
     """My custom model."""
 
     name: str
```

### Comparing `pydantic-kedro-0.7.0/README.md` & `pydantic-kedro-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ## Direct Dataset Usage
 
 This example works for "pure", JSON-safe Pydantic models via
 `PydanticJsonDataset`:
 
 ```python
 from pydantic import BaseModel
+# from pydantic.v1 import BaseModel  # Pydantic V2
 from pydantic_kedro import PydanticJsonDataset
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
 
     x: int
@@ -57,15 +58,15 @@
 
 You can also use `pydantic-kedro` as a generic saving and loading engine for
 Pydantic models:
 
 ```python
 from tempfile import TemporaryDirectory
 
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 from pydantic_kedro import load_model, save_model
 
 class MyModel(BaseModel):
     """My custom model."""
 
     name: str
```

### Comparing `pydantic-kedro-0.7.0/docs/arbitrary_types.md` & `pydantic-kedro-0.8.0/docs/arbitrary_types.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 [PydanticZipDataset][pydantic_kedro.PydanticZipDataset].
 
 ## Usage Example
 
 ```python
 from tempfile import TemporaryDirectory
 from pydantic import BaseModel
+# from pydantic.v1 import BaseModel  # Pydantic V2
 from pydantic_kedro import PydanticZipDataset
 
 
 class Foo(object):
     """My custom class. NOTE: this is not a Pydantic model!"""
 
     def __init__(self, foo):
@@ -88,14 +89,15 @@
 
 Here's a example for [pandas](https://pandas.pydata.org/) and Pydantic V1:
 
 ```python
 import pandas as pd
 from kedro_datasets.pandas import ParquetDataset
 from pydantic import validator
+# from pydantic.v1 import validator  # Pydantic V2
 from pydantic_kedro import ArbModel, PydanticZipDataset
 
 
 class MyPandasModel(ArbModel):
     """Model that saves a dataframe, along with some other data."""
 
     class Config:
```

### Comparing `pydantic-kedro-0.7.0/docs/implementation_details.md` & `pydantic-kedro-0.8.0/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/docs/index.md` & `pydantic-kedro-0.8.0/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
  filepath: folder/my_model
 ```
 
 Then use it as usual within your Kedro pipelines:
 
 ```python
 from pydantic import BaseModel
+# from pydantic.v1 import BaseModel  # Pydantic V2 
 from kedro.pipeline import node
 
 class SomeModel(BaseModel):
     """My custom model."""
 
     name: str
 
@@ -81,14 +82,15 @@
 If you have a JSON-safe Pydantic model, you can use a
 [PydanticJsonDataset][pydantic_kedro.PydanticJsonDataset]
 or [PydanticYamlDataset][pydantic_kedro.PydanticYamlDataset]
 to save your model to any `fsspec`-supported location:
 
 ```python
 from pydantic import BaseModel
+# from pydantic.v1 import BaseModel  # Pydantic V2
 from pydantic_kedro import PydanticJsonDataset
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
 
     x: int
```

### Comparing `pydantic-kedro-0.7.0/docs/standalone_usage.md` & `pydantic-kedro-0.8.0/docs/standalone_usage.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 ## Pure Example
 
 ```python
 from tempfile import TemporaryDirectory
 
 from pydantic import BaseModel
+# from pydantic.v1 import BaseModel  # Pydantic V2
 from pydantic_kedro import load_model, save_model
 
 class MyModel(BaseModel):
     """My custom model."""
 
     name: str
```

### Comparing `pydantic-kedro-0.7.0/mkdocs.yml` & `pydantic-kedro-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/pyproject.toml` & `pydantic-kedro-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 dependencies = [
-    "pydantic>=1.10.0,<2",   # TODO
-    "pydantic-yaml>=1.1.2",
+    "pydantic>=1.10.0,<3",   # WIP
+    "pydantic-yaml>=1.3.0",
     "ruamel-yaml<0.18",      # Current limitation
     "kedro>=0.19.3,<0.20",
     "kedro-datasets>=2.1.0",
     "fsspec",
 ]
 urls = { github = "https://github.com/NowanIlfideme/pydantic-kedro" }
 
@@ -68,23 +68,25 @@
 version = { attr = "pydantic_kedro.version.__version__" }
 
 [tool.setuptools_scm]
 
 [tool.ruff]
 line-length = 105
 src = ["src"]
+
+[tool.ruff.lint]
 select = [
     "E", # pycodestyle
     "F", # pyflakes
     # "UP", # pyupgrade
     "D", # pydocstyle
 ]
 ignore = ["D203", "D213"] # conflicting
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 
 [tool.black]
 line-length = 105
 target-version = ['py39']
 
@@ -118,7 +120,11 @@
     "fsspec.*",
     "cloudpickle",
     "fusepy",
     "ruamel.*",
     "kedro_datasets.*",
 ]
 ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = ["pydantic.v1"]
+ignore_missing_imports = true
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/__init__.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/_dict_io.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/_dict_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for reading/writing from dicts."""
 
 from contextlib import AbstractContextManager
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Type, Union
 
-from pydantic import BaseModel
+from pydantic_kedro._pydantic import BaseModel
 
 from ._internals import import_string
 
 KLS_MARK_STR = "class"
 
 
 def get_kls_path(pyd_kls: Type[BaseModel]) -> str:
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/_internals.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/_internals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Functions for internal use."""
 
 from typing import Any, Callable, Dict, Type
 
-from kedro_datasets.pickle.pickle_dataset import PickleDataset
 from kedro.io.core import AbstractDataset
-from pydantic import BaseModel, create_model
+from kedro_datasets.pickle.pickle_dataset import PickleDataset
+
+from ._pydantic import BaseModel, create_model
 
 KLS_MARK_STR = "class"
 
 
 def import_string(dotted_path: str) -> Any:
     """Import the object from the string. Supports nested classes.
 
@@ -118,15 +119,15 @@
 
     return PickleDataset
 
 
 def create_expanded_model(model: BaseModel) -> BaseModel:
     """Create an 'expanded' model with additional metadata."""
     pyd_kls = type(model)
-    if KLS_MARK_STR in pyd_kls.__fields__.keys():
+    if KLS_MARK_STR in pyd_kls.__fields__.keys():  # type: ignore
         raise ValueError(f"Marker {KLS_MARK_STR!r} already exists as a field; can't dump model.")
     pyd_kls_path = f"{pyd_kls.__module__}.{pyd_kls.__qualname__}"
 
     field_defs = {KLS_MARK_STR: (str, pyd_kls_path)}
 
     tmp_kls = create_model(  # type: ignore
         pyd_kls.__name__,
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/_local_caching.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/_local_caching.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/auto.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Generic Kedro dataset."""
 
 from typing import Any, Dict, Literal, Union
 
 import fsspec
 from fsspec import AbstractFileSystem
 from kedro.io.core import AbstractDataset, get_protocol_and_path
-from pydantic import BaseModel
+
+from pydantic_kedro._pydantic import BaseModel
 
 from .folder import PydanticFolderDataset
 from .json import PydanticJsonDataset
 from .yaml import PydanticYamlDataset
 from .zip import PydanticZipDataset
 
 __all__ = ["PydanticAutoDataset"]
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from uuid import uuid4
 
 import fsspec
 from fsspec import AbstractFileSystem
 from fsspec.core import strip_protocol
 from fsspec.implementations.local import LocalFileSystem
 from kedro.io.core import AbstractDataset, parse_dataset_definition
-from pydantic import BaseConfig, BaseModel, Extra, Field
 
 from pydantic_kedro._dict_io import PatchPydanticIter, dict_to_model
 from pydantic_kedro._internals import get_kedro_default, get_kedro_map, import_string
 from pydantic_kedro._local_caching import get_cache_dir
+from pydantic_kedro._pydantic import BaseConfig, BaseModel, Extra, Field
 
 __all__ = ["PydanticFolderDataset"]
 
 
 DATA_PLACEHOLDER = "__DATA_PLACEHOLDER__"
 
 JsonPath = str  # not a "real" JSON Path, but just `.`-separated
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import warnings
 from pathlib import PurePosixPath
 from typing import Any, Dict, no_type_check
 
 import fsspec
 from fsspec import AbstractFileSystem
 from kedro.io.core import AbstractDataset, get_filepath_str, get_protocol_and_path
-from pydantic import BaseModel
 
 from pydantic_kedro._dict_io import PatchPydanticIter, dict_to_model
+from pydantic_kedro._pydantic import BaseModel
 
 
 class PydanticJsonDataset(AbstractDataset[BaseModel, BaseModel]):
     """Dataset for saving/loading Pydantic models, based on JSON.
 
     Please note that the Pydantic model must be JSON-serializable.
     That means the fields are "pure" Pydantic fields,
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/yaml.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/yaml.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pathlib import PurePosixPath
 from typing import Any, Dict, no_type_check
 
 import fsspec
 import ruamel.yaml as yaml
 from fsspec import AbstractFileSystem
 from kedro.io.core import AbstractDataset, get_filepath_str, get_protocol_and_path
-from pydantic import BaseModel
 from pydantic_yaml import to_yaml_file
 
 from pydantic_kedro._dict_io import PatchPydanticIter, dict_to_model
+from pydantic_kedro._pydantic import BaseModel
 
 
 class PydanticYamlDataset(AbstractDataset[BaseModel, BaseModel]):
     """Dataset for saving/loading Pydantic models, based on YAML.
 
     Please note that the Pydantic model must be JSON-serializable.
     That means the fields are "pure" Pydantic fields,
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/datasets/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from tempfile import TemporaryDirectory
 from typing import Any, Dict
 from uuid import uuid4
 
 import fsspec
 from fsspec.implementations.zip import ZipFileSystem
 from kedro.io.core import AbstractDataset
-from pydantic import BaseModel
 
 from pydantic_kedro._local_caching import get_cache_dir
+from pydantic_kedro._pydantic import BaseModel
 
 from .folder import PydanticFolderDataset
 
 
 class PydanticZipDataset(AbstractDataset[BaseModel, BaseModel]):
     """Dataset for saving/loading Pydantic models, based on saving sub-datasets in a ZIP file.
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/models.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Models to use as base classes."""
 
 from typing import Callable, Dict, Type
 
-from kedro_datasets.pickle.pickle_dataset import PickleDataset
 from kedro.io import AbstractDataset
-from pydantic import BaseConfig, BaseModel
+from kedro_datasets.pickle.pickle_dataset import PickleDataset
+
+from pydantic_kedro._pydantic import BaseConfig, BaseModel
 
 
 def _kedro_default(x: str) -> PickleDataset:
     """Definition of default dataset."""
     return PickleDataset(filepath=x)
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro/utils.py` & `pydantic-kedro-0.8.0/src/pydantic_kedro/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utilities for reading/writing objects."""
 
 from typing import Literal, Type, TypeVar
 
 from kedro.io.core import AbstractDataset
-from pydantic import BaseModel
 
+from pydantic_kedro._pydantic import BaseModel
 from pydantic_kedro.datasets.auto import PydanticAutoDataset
 from pydantic_kedro.datasets.folder import PydanticFolderDataset
 from pydantic_kedro.datasets.json import PydanticJsonDataset
 from pydantic_kedro.datasets.yaml import PydanticYamlDataset
 from pydantic_kedro.datasets.zip import PydanticZipDataset
 
 __all__ = ["load_model", "save_model"]
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.7.0
+Version: 0.8.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,16 +31,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic<2,>=1.10.0
-Requires-Dist: pydantic-yaml>=1.1.2
+Requires-Dist: pydantic<3,>=1.10.0
+Requires-Dist: pydantic-yaml>=1.3.0
 Requires-Dist: ruamel-yaml<0.18
 Requires-Dist: kedro<0.20,>=0.19.3
 Requires-Dist: kedro-datasets>=2.1.0
 Requires-Dist: fsspec
 Provides-Extra: dev
 Requires-Dist: setuptools>=61.0.0; extra == "dev"
 Requires-Dist: setuptools-scm[toml]>=6.2; extra == "dev"
@@ -91,14 +91,15 @@
 ## Direct Dataset Usage
 
 This example works for "pure", JSON-safe Pydantic models via
 `PydanticJsonDataset`:
 
 ```python
 from pydantic import BaseModel
+# from pydantic.v1 import BaseModel  # Pydantic V2
 from pydantic_kedro import PydanticJsonDataset
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
 
     x: int
@@ -120,15 +121,15 @@
 
 You can also use `pydantic-kedro` as a generic saving and loading engine for
 Pydantic models:
 
 ```python
 from tempfile import TemporaryDirectory
 
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 from pydantic_kedro import load_model, save_model
 
 class MyModel(BaseModel):
     """My custom model."""
 
     name: str
```

### Comparing `pydantic-kedro-0.7.0/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.8.0/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .markdownlint.yaml
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 README.md
+env-v1.yml
 environment.yml
 mkdocs.yml
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-testing.yml
@@ -16,14 +17,15 @@
 docs/index.md
 docs/reference.md
 docs/standalone_usage.md
 src/pydantic_kedro/__init__.py
 src/pydantic_kedro/_dict_io.py
 src/pydantic_kedro/_internals.py
 src/pydantic_kedro/_local_caching.py
+src/pydantic_kedro/_pydantic.py
 src/pydantic_kedro/models.py
 src/pydantic_kedro/py.typed
 src/pydantic_kedro/utils.py
 src/pydantic_kedro/version.py
 src/pydantic_kedro.egg-info/PKG-INFO
 src/pydantic_kedro.egg-info/SOURCES.txt
 src/pydantic_kedro.egg-info/dependency_links.txt
```

### Comparing `pydantic-kedro-0.7.0/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.8.0/src/test/catalogs/test_basic_catalog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Minimal tests for the Kedro catalog."""
 
 import os
 from pathlib import Path
 
 from kedro.config import OmegaConfigLoader
 from kedro.io import DataCatalog
-from pydantic import BaseModel
 
 from pydantic_kedro import PydanticJsonDataset
+from pydantic_kedro._pydantic import BaseModel
 
 local_dir = Path(__file__).parent
 
 
 class MyPureModel(BaseModel):
     """Your custom Pydantic model with JSON-safe fields."""
```

### Comparing `pydantic-kedro-0.7.0/src/test/test_auto.py` & `pydantic-kedro-0.8.0/src/test/test_auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Specialized tests for `PydanticAutoDataset`."""
 
-from pydantic import BaseModel
-
+from pydantic_kedro._pydantic import BaseModel
 from pydantic_kedro import PydanticAutoDataset, PydanticJsonDataset, PydanticZipDataset
 
 
 class MyModel(BaseModel):
     """My model."""
 
     x: str
```

### Comparing `pydantic-kedro-0.7.0/src/test/test_docs_standalone.py` & `pydantic-kedro-0.8.0/src/test/test_docs_standalone.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/src/test/test_ds_extended.py` & `pydantic-kedro-0.8.0/src/test/test_ds_extended.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/src/test/test_ds_pandas.py` & `pydantic-kedro-0.8.0/src/test/test_ds_pandas.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/src/test/test_ds_simple.py` & `pydantic-kedro-0.8.0/src/test/test_ds_simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests the datasets on a simple model."""
 
 from typing import Optional
 
 import pytest
 from kedro.io.core import AbstractDataset
-from pydantic import BaseModel
+from pydantic_kedro._pydantic import BaseModel
 
 from pydantic_kedro import (
     PydanticAutoDataset,
     PydanticFolderDataset,
     PydanticJsonDataset,
     PydanticYamlDataset,
     PydanticZipDataset,
```

### Comparing `pydantic-kedro-0.7.0/src/test/test_ds_spark.py` & `pydantic-kedro-0.8.0/src/test/test_ds_spark.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.7.0/src/test/test_inheritance.py` & `pydantic-kedro-0.8.0/src/test/test_inheritance.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Type, Union
 
 import pandas as pd
 import pytest
 from kedro_datasets.pandas.csv_dataset import CSVDataset
 from kedro_datasets.pandas.parquet_dataset import ParquetDataset
 from kedro_datasets.pickle.pickle_dataset import PickleDataset
-from pydantic import BaseModel
 
 from pydantic_kedro import PydanticFolderDataset
+from pydantic_kedro._pydantic import BaseModel
 
 dfx = pd.DataFrame([[1, 2, 3]], columns=["a", "b", "c"])
 
 
 def csv_ds(path: str) -> CSVDataset:
     """Create a CSV dataset."""
     return CSVDataset(filepath=path, save_args=dict(index=False), load_args=dict())
```

### Comparing `pydantic-kedro-0.7.0/src/test/test_nested_subtypes.py` & `pydantic-kedro-0.8.0/src/test/test_nested_subtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for values which are subclasses of the Pydantic field types."""
 
 from abc import abstractmethod
 from typing import Dict, List, Literal
 
 import pytest
-from pydantic import BaseModel
 
+from pydantic_kedro._pydantic import BaseModel
 from pydantic_kedro import load_model, save_model
 
 
 class AbstractBaz(BaseModel):
     """Abstract base model which is used as an interface.
 
     This can occur with ANY model type, however with abstract models it's much more apparent.
@@ -56,15 +56,15 @@
 @pytest.mark.parametrize("obj", [AlwaysBaz(foo="always"), CopyBaz(foo="copy")])
 def test_nested_subclass(
     obj: AbstractBaz, format: Literal["auto", "zip", "folder", "yaml", "json"], tmpdir: str
 ):
     """Test round-trip of objects with a nested subclass."""
     # Initial round-trip (should always work)
     save_model(obj, f"{tmpdir}/obj", format=format)
-    obj2 = load_model(f"{tmpdir}/obj", AbstractBaz)
+    obj2 = load_model(f"{tmpdir}/obj", AbstractBaz)  # type: ignore[type-abstract]
     assert obj.foo == obj2.foo
     assert obj.get_baz() == obj2.get_baz()
     # Nested round-trip (should also always work, but is more diffictult)
     nest = Bazzifier(maker=obj)
     save_model(nest, f"{tmpdir}/nest", format=format)
     nest2 = load_model(f"{tmpdir}/nest", Bazzifier)
     assert nest.maker == nest2.maker
```

### Comparing `pydantic-kedro-0.7.0/src/test/test_strict.py` & `pydantic-kedro-0.8.0/src/test/test_strict.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test strict models and BaseSettings subclasses."""
 
 import pytest
-from pydantic import BaseModel, BaseSettings
 from typing_extensions import Literal
 
 from pydantic_kedro import load_model, save_model
+from pydantic_kedro._pydantic import BaseModel, BaseSettings
 
 
 class ExSettings(BaseSettings):
     """Settings class."""
 
     val: str
```

