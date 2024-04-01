# Comparing `tmp/feud-0.3.1.tar.gz` & `tmp/feud-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feud-0.3.1.tar", max compression
+gzip compressed data, was "feud-0.3.2.tar", max compression
```

## Comparing `feud-0.3.1.tar` & `feud-0.3.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     8386 2024-01-12 19:20:00.933208 feud-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1096 2024-01-12 19:20:00.933208 feud-0.3.1/LICENSE
--rw-r--r--   0        0        0      473 2024-01-12 19:20:00.933208 feud-0.3.1/Makefile
--rw-r--r--   0        0        0    33195 2024-01-12 19:20:00.933208 feud-0.3.1/README.md
--rw-r--r--   0        0        0      598 2024-01-12 19:20:00.949208 feud-0.3.1/feud/__init__.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.949208 feud-0.3.1/feud/_internal/__init__.py
--rw-r--r--   0        0        0    14672 2024-01-12 19:20:00.949208 feud-0.3.1/feud/_internal/_command.py
--rw-r--r--   0        0        0     3024 2024-01-12 19:20:00.949208 feud-0.3.1/feud/_internal/_decorators.py
--rw-r--r--   0        0        0     2618 2024-01-12 19:20:00.949208 feud-0.3.1/feud/_internal/_docstring.py
--rw-r--r--   0        0        0     1290 2024-01-12 19:20:00.953208 feud-0.3.1/feud/_internal/_group.py
--rw-r--r--   0        0        0     4960 2024-01-12 19:20:00.953208 feud-0.3.1/feud/_internal/_inflect.py
--rw-r--r--   0        0        0     5035 2024-01-12 19:20:00.953208 feud-0.3.1/feud/_internal/_metaclass.py
--rw-r--r--   0        0        0     3598 2024-01-12 19:20:00.953208 feud-0.3.1/feud/_internal/_sections.py
--rw-r--r--   0        0        0      266 2024-01-12 19:20:00.953208 feud-0.3.1/feud/_internal/_types/__init__.py
--rw-r--r--   0        0        0    15085 2024-01-12 19:20:00.953208 feud-0.3.1/feud/_internal/_types/click.py
--rw-r--r--   0        0        0      771 2024-01-12 19:20:00.953208 feud-0.3.1/feud/_internal/_types/defaults.py
--rw-r--r--   0        0        0      477 2024-01-12 19:20:00.953208 feud-0.3.1/feud/click/__init__.py
--rw-r--r--   0        0        0     1117 2024-01-12 19:20:00.953208 feud-0.3.1/feud/click/context.py
--rw-r--r--   0        0        0     4976 2024-01-12 19:20:00.953208 feud-0.3.1/feud/config.py
--rw-r--r--   0        0        0    13037 2024-01-12 19:20:00.953208 feud-0.3.1/feud/core/__init__.py
--rw-r--r--   0        0        0     3764 2024-01-12 19:20:00.953208 feud-0.3.1/feud/core/command.py
--rw-r--r--   0        0        0    24069 2024-01-12 19:20:00.953208 feud-0.3.1/feud/core/group.py
--rw-r--r--   0        0        0     9602 2024-01-12 19:20:00.953208 feud-0.3.1/feud/decorators.py
--rw-r--r--   0        0        0      619 2024-01-12 19:20:00.953208 feud-0.3.1/feud/exceptions.py
--rw-r--r--   0        0        0      625 2024-01-12 19:20:00.953208 feud-0.3.1/feud/typing/__init__.py
--rw-r--r--   0        0        0     2221 2024-01-12 19:20:00.953208 feud-0.3.1/feud/typing/custom.py
--rw-r--r--   0        0        0     2447 2024-01-12 19:20:00.953208 feud-0.3.1/feud/typing/pydantic.py
--rw-r--r--   0        0        0     2027 2024-01-12 19:20:00.953208 feud-0.3.1/feud/typing/pydantic_extra_types.py
--rw-r--r--   0        0        0      988 2024-01-12 19:20:00.953208 feud-0.3.1/feud/typing/stdlib.py
--rw-r--r--   0        0        0      626 2024-01-12 19:20:00.953208 feud-0.3.1/feud/typing/typing.py
--rw-r--r--   0        0        0     2754 2024-01-12 19:20:00.953208 feud-0.3.1/feud/version.py
--rw-r--r--   0        0        0      300 2024-01-12 19:20:00.953208 feud-0.3.1/make/__init__.py
--rw-r--r--   0        0        0      504 2024-01-12 19:20:00.953208 feud-0.3.1/make/cov.py
--rw-r--r--   0        0        0      883 2024-01-12 19:20:00.953208 feud-0.3.1/make/docs.py
--rw-r--r--   0        0        0     1028 2024-01-12 19:20:00.953208 feud-0.3.1/make/lint.py
--rw-r--r--   0        0        0     1111 2024-01-12 19:20:00.953208 feud-0.3.1/make/release.py
--rw-r--r--   0        0        0     1111 2024-01-12 19:20:00.953208 feud-0.3.1/make/tests.py
--rw-r--r--   0        0        0     7168 2024-01-12 19:20:00.953208 feud-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1859 2024-01-12 19:20:00.953208 feud-0.3.1/tasks.py
--rw-r--r--   0        0        0        0 2024-01-12 19:20:00.953208 feud-0.3.1/tests/.gitkeep
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/__init__.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_click/__init__.py
--rw-r--r--   0        0        0      568 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_click/test_context.py
--rw-r--r--   0        0        0     4668 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_config.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_core/__init__.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_core/fixtures/__init__.py
--rw-r--r--   0        0        0     1383 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_core/fixtures/module.py
--rw-r--r--   0        0        0    11115 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_core/test_command.py
--rw-r--r--   0        0        0    35939 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_core/test_group.py
--rw-r--r--   0        0        0    22436 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_core/test_run.py
--rw-r--r--   0        0        0     9858 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_decorators.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/__init__.py
--rw-r--r--   0        0        0     3811 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_command.py
--rw-r--r--   0        0        0     5432 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_decorators.py
--rw-r--r--   0        0        0     6636 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_docstring.py
--rw-r--r--   0        0        0     3806 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_metaclass.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/__init__.py
--rw-r--r--   0        0        0      520 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/conftest.py
--rw-r--r--   0        0        0      216 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/__init__.py
--rw-r--r--   0        0        0     1303 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/conftest.py
--rw-r--r--   0        0        0     1044 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_custom.py
--rw-r--r--   0        0        0     3203 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_literal.py
--rw-r--r--   0        0        0     6293 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic.py
--rw-r--r--   0        0        0     1474 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic_extra_types.py
--rw-r--r--   0        0        0     1813 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_stdlib.py
--rw-r--r--   0        0        0     2313 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_typing.py
--rw-r--r--   0        0        0     4573 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_is_collection_type.py
--rw-r--r--   0        0        0     1220 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_metavars.py
--rw-r--r--   0        0        0      756 2024-01-12 19:20:00.953208 feud-0.3.1/tests/unit/test_version.py
--rw-r--r--   0        0        0      685 2024-01-12 19:20:00.953208 feud-0.3.1/tox.ini
--rw-r--r--   0        0        0    35107 1970-01-01 00:00:00.000000 feud-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     8586 2024-04-01 19:00:42.758205 feud-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1096 2024-04-01 19:00:42.758205 feud-0.3.2/LICENSE
+-rw-r--r--   0        0        0      473 2024-04-01 19:00:42.758205 feud-0.3.2/Makefile
+-rw-r--r--   0        0        0    33128 2024-04-01 19:00:42.758205 feud-0.3.2/README.md
+-rw-r--r--   0        0        0      598 2024-04-01 19:00:42.778205 feud-0.3.2/feud/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/__init__.py
+-rw-r--r--   0        0        0    14672 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_command.py
+-rw-r--r--   0        0        0     3024 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_decorators.py
+-rw-r--r--   0        0        0     2618 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_docstring.py
+-rw-r--r--   0        0        0     1290 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_group.py
+-rw-r--r--   0        0        0     4960 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_inflect.py
+-rw-r--r--   0        0        0     5035 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_metaclass.py
+-rw-r--r--   0        0        0     3598 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_sections.py
+-rw-r--r--   0        0        0      266 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_types/__init__.py
+-rw-r--r--   0        0        0    15085 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_types/click.py
+-rw-r--r--   0        0        0      771 2024-04-01 19:00:42.778205 feud-0.3.2/feud/_internal/_types/defaults.py
+-rw-r--r--   0        0        0      477 2024-04-01 19:00:42.778205 feud-0.3.2/feud/click/__init__.py
+-rw-r--r--   0        0        0     1117 2024-04-01 19:00:42.778205 feud-0.3.2/feud/click/context.py
+-rw-r--r--   0        0        0     4976 2024-04-01 19:00:42.778205 feud-0.3.2/feud/config.py
+-rw-r--r--   0        0        0    13037 2024-04-01 19:00:42.778205 feud-0.3.2/feud/core/__init__.py
+-rw-r--r--   0        0        0     3764 2024-04-01 19:00:42.778205 feud-0.3.2/feud/core/command.py
+-rw-r--r--   0        0        0    24069 2024-04-01 19:00:42.778205 feud-0.3.2/feud/core/group.py
+-rw-r--r--   0        0        0     9602 2024-04-01 19:00:42.778205 feud-0.3.2/feud/decorators.py
+-rw-r--r--   0        0        0      619 2024-04-01 19:00:42.778205 feud-0.3.2/feud/exceptions.py
+-rw-r--r--   0        0        0      625 2024-04-01 19:00:42.778205 feud-0.3.2/feud/typing/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-01 19:00:42.778205 feud-0.3.2/feud/typing/custom.py
+-rw-r--r--   0        0        0     2447 2024-04-01 19:00:42.778205 feud-0.3.2/feud/typing/pydantic.py
+-rw-r--r--   0        0        0     2027 2024-04-01 19:00:42.778205 feud-0.3.2/feud/typing/pydantic_extra_types.py
+-rw-r--r--   0        0        0      988 2024-04-01 19:00:42.778205 feud-0.3.2/feud/typing/stdlib.py
+-rw-r--r--   0        0        0      626 2024-04-01 19:00:42.778205 feud-0.3.2/feud/typing/typing.py
+-rw-r--r--   0        0        0     2754 2024-04-01 19:00:42.778205 feud-0.3.2/feud/version.py
+-rw-r--r--   0        0        0      300 2024-04-01 19:00:42.778205 feud-0.3.2/make/__init__.py
+-rw-r--r--   0        0        0      504 2024-04-01 19:00:42.778205 feud-0.3.2/make/cov.py
+-rw-r--r--   0        0        0      883 2024-04-01 19:00:42.778205 feud-0.3.2/make/docs.py
+-rw-r--r--   0        0        0     1028 2024-04-01 19:00:42.778205 feud-0.3.2/make/lint.py
+-rw-r--r--   0        0        0     1111 2024-04-01 19:00:42.778205 feud-0.3.2/make/release.py
+-rw-r--r--   0        0        0     1111 2024-04-01 19:00:42.778205 feud-0.3.2/make/tests.py
+-rw-r--r--   0        0        0     7168 2024-04-01 19:00:42.778205 feud-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1859 2024-04-01 19:00:42.778205 feud-0.3.2/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:00:42.778205 feud-0.3.2/tests/.gitkeep
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_click/__init__.py
+-rw-r--r--   0        0        0      568 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_click/test_context.py
+-rw-r--r--   0        0        0     4668 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_config.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_core/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_core/fixtures/__init__.py
+-rw-r--r--   0        0        0     1383 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_core/fixtures/module.py
+-rw-r--r--   0        0        0    11115 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_core/test_command.py
+-rw-r--r--   0        0        0    35939 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_core/test_group.py
+-rw-r--r--   0        0        0    22436 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_core/test_run.py
+-rw-r--r--   0        0        0     9858 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_decorators.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/__init__.py
+-rw-r--r--   0        0        0     3811 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_command.py
+-rw-r--r--   0        0        0     5432 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_decorators.py
+-rw-r--r--   0        0        0     6636 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_docstring.py
+-rw-r--r--   0        0        0     3806 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_metaclass.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/conftest.py
+-rw-r--r--   0        0        0      216 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/conftest.py
+-rw-r--r--   0        0        0     1044 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_custom.py
+-rw-r--r--   0        0        0     3203 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_literal.py
+-rw-r--r--   0        0        0     6293 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic.py
+-rw-r--r--   0        0        0     1474 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic_extra_types.py
+-rw-r--r--   0        0        0     1813 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_stdlib.py
+-rw-r--r--   0        0        0     2313 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_typing.py
+-rw-r--r--   0        0        0     4573 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_is_collection_type.py
+-rw-r--r--   0        0        0     1220 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_metavars.py
+-rw-r--r--   0        0        0      756 2024-04-01 19:00:42.778205 feud-0.3.2/tests/unit/test_version.py
+-rw-r--r--   0        0        0      685 2024-04-01 19:00:42.778205 feud-0.3.2/tox.ini
+-rw-r--r--   0        0        0    35040 1970-01-01 00:00:00.000000 feud-0.3.2/PKG-INFO
```

### Comparing `feud-0.3.1/CHANGELOG.md` & `feud-0.3.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [v0.3.2](https://github.com/eonu/feud/releases/tag/v0.3.2) - 2024-04-01
+
+### Documentation
+
+- specify virtual env location in `.readthedocs.yaml` ([#143](https://github.com/eonu/feud/issues/143))
+
 ## [v0.3.1](https://github.com/eonu/feud/releases/tag/v0.3.1) - 2024-01-12
 
 ### Documentation
 
 - fix broken core/command docs links ([#139](https://github.com/eonu/feud/issues/139))
 - update package description ([#141](https://github.com/eonu/feud/issues/141))
```

### Comparing `feud-0.3.1/LICENSE` & `feud-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/README.md` & `feud-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,17 +42,14 @@
     <a href="#contributing">Contributing</a> ·
     <a href="#licensing">Licensing</a>
   </sup>
 </p>
 
 ## About
 
-> [!WARNING]  
-> _Writing command-line interfaces can get messy!_
-
 Designing a _good_ CLI can quickly spiral into chaos without the help of
 an intuitive CLI framework.
 
 **Feud builds on [Click](https://click.palletsprojects.com/en/8.1.x/) for
 argument parsing, along with [Pydantic](https://docs.pydantic.dev/latest/)
 for typing, to make CLI building a breeze.**
```

### Comparing `feud-0.3.1/feud/__init__.py` & `feud-0.3.2/feud/__init__.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_command.py` & `feud-0.3.2/feud/_internal/_command.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_decorators.py` & `feud-0.3.2/feud/_internal/_decorators.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_docstring.py` & `feud-0.3.2/feud/_internal/_docstring.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_group.py` & `feud-0.3.2/feud/_internal/_group.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_inflect.py` & `feud-0.3.2/feud/_internal/_inflect.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_metaclass.py` & `feud-0.3.2/feud/_internal/_metaclass.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_sections.py` & `feud-0.3.2/feud/_internal/_sections.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_types/click.py` & `feud-0.3.2/feud/_internal/_types/click.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/_internal/_types/defaults.py` & `feud-0.3.2/feud/_internal/_types/defaults.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/click/context.py` & `feud-0.3.2/feud/click/context.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/config.py` & `feud-0.3.2/feud/config.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/core/__init__.py` & `feud-0.3.2/feud/core/__init__.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/core/command.py` & `feud-0.3.2/feud/core/command.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/core/group.py` & `feud-0.3.2/feud/core/group.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/decorators.py` & `feud-0.3.2/feud/decorators.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/exceptions.py` & `feud-0.3.2/feud/exceptions.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/typing/__init__.py` & `feud-0.3.2/feud/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/typing/custom.py` & `feud-0.3.2/feud/typing/custom.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/typing/pydantic.py` & `feud-0.3.2/feud/typing/pydantic.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/typing/pydantic_extra_types.py` & `feud-0.3.2/feud/typing/pydantic_extra_types.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/typing/stdlib.py` & `feud-0.3.2/feud/typing/stdlib.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/typing/typing.py` & `feud-0.3.2/feud/typing/typing.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/feud/version.py` & `feud-0.3.2/feud/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
     FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
     DEALINGS IN THE SOFTWARE.
 """
 
 __all__ = ["VERSION", "version_info"]
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 
 def version_info() -> str:
     """Return complete version information for Feud and its dependencies."""
     import importlib.metadata as importlib_metadata
     import platform
     import sys
```

### Comparing `feud-0.3.1/make/docs.py` & `feud-0.3.2/make/docs.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/make/lint.py` & `feud-0.3.2/make/lint.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/make/release.py` & `feud-0.3.2/make/release.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/make/tests.py` & `feud-0.3.2/make/tests.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/pyproject.toml` & `feud-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feud"
-version = "0.3.1"
+version = "0.3.2"
 license = "MIT"
 authors = ["Edwin Onuonga <ed@eonu.net>"]
 maintainers = ["Edwin Onuonga <ed@eonu.net>"]
 description = "Build powerful CLIs with simple idiomatic Python, driven by type hints. Not all arguments are bad."
 readme = "README.md"
 homepage = "https://github.com/eonu/feud"
 repository = "https://github.com/eonu/feud"
```

### Comparing `feud-0.3.1/tasks.py` & `feud-0.3.2/tasks.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_click/test_context.py` & `feud-0.3.2/tests/unit/test_click/test_context.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_config.py` & `feud-0.3.2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_core/fixtures/module.py` & `feud-0.3.2/tests/unit/test_core/fixtures/module.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_core/test_command.py` & `feud-0.3.2/tests/unit/test_core/test_command.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_core/test_group.py` & `feud-0.3.2/tests/unit/test_core/test_group.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_core/test_run.py` & `feud-0.3.2/tests/unit/test_core/test_run.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_decorators.py` & `feud-0.3.2/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_command.py` & `feud-0.3.2/tests/unit/test_internal/test_command.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_decorators.py` & `feud-0.3.2/tests/unit/test_internal/test_decorators.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_docstring.py` & `feud-0.3.2/tests/unit/test_internal/test_docstring.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_metaclass.py` & `feud-0.3.2/tests/unit/test_internal/test_metaclass.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/conftest.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/conftest.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/conftest.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/conftest.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_custom.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_custom.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_literal.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_literal.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic_extra_types.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_pydantic_extra_types.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_stdlib.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_typing.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_get_click_type/test_typing.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_is_collection_type.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_is_collection_type.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_internal/test_types/test_click/test_metavars.py` & `feud-0.3.2/tests/unit/test_internal/test_types/test_click/test_metavars.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tests/unit/test_version.py` & `feud-0.3.2/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/tox.ini` & `feud-0.3.2/tox.ini`

 * *Files identical despite different names*

### Comparing `feud-0.3.1/PKG-INFO` & `feud-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feud
-Version: 0.3.1
+Version: 0.3.2
 Summary: Build powerful CLIs with simple idiomatic Python, driven by type hints. Not all arguments are bad.
 Home-page: https://github.com/eonu/feud
 License: MIT
 Keywords: python,cli,terminal,command-line,typed,docstrings,typehints,pydantic,click
 Author: Edwin Onuonga
 Author-email: ed@eonu.net
 Maintainer: Edwin Onuonga
@@ -86,17 +86,14 @@
     <a href="#contributing">Contributing</a> ·
     <a href="#licensing">Licensing</a>
   </sup>
 </p>
 
 ## About
 
-> [!WARNING]  
-> _Writing command-line interfaces can get messy!_
-
 Designing a _good_ CLI can quickly spiral into chaos without the help of
 an intuitive CLI framework.
 
 **Feud builds on [Click](https://click.palletsprojects.com/en/8.1.x/) for
 argument parsing, along with [Pydantic](https://docs.pydantic.dev/latest/)
 for typing, to make CLI building a breeze.**
```

