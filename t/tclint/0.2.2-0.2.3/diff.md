# Comparing `tmp/tclint-0.2.2.tar.gz` & `tmp/tclint-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclint-0.2.2.tar", last modified: Sat Mar 16 21:19:46 2024, max compression
+gzip compressed data, was "tclint-0.2.3.tar", last modified: Mon Apr  1 21:49:47 2024, max compression
```

## Comparing `tclint-0.2.2.tar` & `tclint-0.2.3.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.731045 tclint-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-16 21:19:38.000000 tclint-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.719045 tclint-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.719045 tclint-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-16 21:19:38.000000 tclint-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-16 21:19:38.000000 tclint-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-16 21:19:38.000000 tclint-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-16 21:19:38.000000 tclint-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-16 21:19:46.731045 tclint-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-16 21:19:38.000000 tclint-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-16 21:19:38.000000 tclint-0.2.2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-16 21:19:38.000000 tclint-0.2.2/dev-constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.723045 tclint-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-16 21:19:38.000000 tclint-0.2.2/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-16 21:19:38.000000 tclint-0.2.2/docs/violations.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-16 21:19:38.000000 tclint-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 21:19:46.731045 tclint-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.719045 tclint-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.723045 tclint-0.2.2/src/tclint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-16 21:19:46.000000 tclint-0.2.2/src/tclint/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25133 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.723045 tclint-0.2.2/src/tclint/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/commands/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27503 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/tclint.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-16 21:19:38.000000 tclint-0.2.2/src/tclint/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.731045 tclint-0.2.2/src/tclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-16 21:19:46.000000 tclint-0.2.2/src/tclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-16 21:19:46.000000 tclint-0.2.2/src/tclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 21:19:46.000000 tclint-0.2.2/src/tclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-16 21:19:46.000000 tclint-0.2.2/src/tclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-16 21:19:46.000000 tclint-0.2.2/src/tclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-16 21:19:46.000000 tclint-0.2.2/src/tclint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.727045 tclint-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:46.731045 tclint-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/backslash-spacing.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/backslash-spacing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/blank-lines.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/blank-lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/clean.tcl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/clean.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/dirty.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/dirty.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/example.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/example.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/expr-format.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/expr-format.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/indent.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/indent.txt
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/indent_lists.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/indent_lists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/lines.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/spaces-in-braces.tcl
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/spaces-in-braces.toml
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/spaces-in-braces.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/special-comments.tcl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/special-comments.txt
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/data/tclint.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)    18244 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-16 21:19:38.000000 tclint-0.2.2/tests/test_tclint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.755031 tclint-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-01 21:49:44.000000 tclint-0.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 21:49:44.000000 tclint-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-01 21:49:44.000000 tclint-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-01 21:49:44.000000 tclint-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-01 21:49:44.000000 tclint-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-01 21:49:47.755031 tclint-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-01 21:49:44.000000 tclint-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-01 21:49:44.000000 tclint-0.2.3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 21:49:44.000000 tclint-0.2.3/dev-constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-01 21:49:44.000000 tclint-0.2.3/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-01 21:49:44.000000 tclint-0.2.3/docs/violations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-01 21:49:44.000000 tclint-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:49:47.755031 tclint-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.751031 tclint-0.2.3/src/tclint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25942 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.751031 tclint-0.2.3/src/tclint/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27503 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/tclint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.755031 tclint-0.2.3/src/tclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.751031 tclint-0.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.755031 tclint-0.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/backslash-spacing.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/backslash-spacing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/blank-lines.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/blank-lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/clean.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/clean.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/dirty.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/dirty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/example.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/expr-format.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/expr-format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent_lists.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent_lists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/lines.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/spaces-in-braces.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/spaces-in-braces.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/spaces-in-braces.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/special-comments.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/special-comments.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/tclint.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_tclint.py
```

### Comparing `tclint-0.2.2/.github/workflows/ci.yml` & `tclint-0.2.3/.github/workflows/ci.yml`

 * *Files 21% similar despite different names*

```diff
@@ -64,9 +64,10 @@
       - name: Lint
         run: |
           pip install flake8 -c dev-constraints.txt
           flake8 --statistics .
 
       - name: Typecheck
         run: |
+          pip install . # need to install package to ensure we get type stubs for deps
           pip install mypy -c dev-constraints.txt
           mypy src
```

### Comparing `tclint-0.2.2/.github/workflows/release.yml` & `tclint-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/LICENSE` & `tclint-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/PKG-INFO` & `tclint-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tclint
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI utility for linting and analyzing Tcl code.
 Author-email: Noah Moroze <me@noahmoroze.com>
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply==3.11
 Requires-Dist: schema==0.7.5
 Requires-Dist: tomli~=2.0.1; python_version < "3.11"
+Requires-Dist: pathspec==0.11.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 
 # tclint &nbsp; [![CI](https://github.com/nmoroze/tclint/actions/workflows/ci.yml/badge.svg)](https://github.com/nmoroze/tclint/actions/workflows/ci.yml)
```

### Comparing `tclint-0.2.2/README.md` & `tclint-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/docs/configuration.md` & `tclint-0.2.3/docs/configuration.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Configuration
 
 `tclint` is configured via a [TOML](https://toml.io/en/) configuration file.
 
 The following example shows all supported fields:
 
 ```toml
-# paths to exclude when searching directories. defaults to empty list.
-exclude = ["ignore_me/", "ignore.tcl"]
+# patterns to exclude when searching directories. defaults to empty list.
+# follows gitignore pattern format: https://git-scm.com/docs/gitignore#_pattern_format
+# the one exception is that a leading "#" character will be automatically escaped
+exclude = ["ignore_me/", "ignore*.tcl", "/ignore_from_here"]
 # lint violations to ignore. defaults to empty list.
 # can also supply an inline table with a path and a list of violations to ignore under that path.
 ignore = [
     "spacing",
     { path = "files_with_bad_indent/", rules = ["indent"] }
 ]
 
@@ -57,16 +59,16 @@
 
 Each configuration field supports at least one command line argument that can be used to override its value. Values supplied using these switches always override values supplied in the config file, with the exception of `--extend-exclude` and `--extend-ignore`, which extends any previously configured list with the supplied values.
 
 ```
 configuration arguments:
   --ignore "rule1, rule2, ..."
   --extend-ignore "rule1, rule2, ..."
-  --exclude "path1, path2, ..."
-  --extend-exclude "path1, path2, ..."
+  --exclude "pattern1, pattern2, ..."
+  --extend-exclude "pattern1, pattern2, ..."
   --style-indent <indent>
   --style-line-length <line_length>
   --style-max-blank-lines <max_blank_lines>
   --style-aligned-sets
   --style-no-aligned-sets
   --style-indent-namespace-eval
   --style-no-indent-namespace-eval
```

### Comparing `tclint-0.2.2/docs/violations.md` & `tclint-0.2.3/docs/violations.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 - [`trailing-whitespace`](#trailing-whitespace)
 - [`blank-lines`](#blank-lines)
 - [`command-args`](#command-args)
 - [`redefined-builtin`](#redefined-builtin)
 - [`backslash-spacing`](#backslash-spacing)
 - [`expr-format`](#expr-format)
 - [`spaces-in-braces`](#spaces-in-braces)
+- [`unbraced-expr`](#unbraced-expr)
+
+Each of these violations is sorted into one of two coarse categories, which can
+be displayed using the `--show-categories` CLI option.
+
+- `func`: violations that may impact the script's functionality
+- `style`: style-related violations with no functional impact
 
 ## `indent`
 
 Source files must be indented consistently. `tclint` requires an additional level of indentation within script arguments (e.g. the body of an `if` or `while` command), as well as for continuations of command arguments.
 
 The one configurable exception is the `namespace eval` command. If `style.indent-namespace-eval` is false, then the body of this command doesn't need an extra level of indentation. The default is true.
 
@@ -124,7 +131,20 @@
     puts $i
 }
 ```
 
 ### Rationale
 
 Consistent formatting enhances readability.
+
+## `unbraced-expr`
+
+Expressions that contain substitutions should be enclosed by braces.
+
+### Rationale
+
+Without braces, the Tcl parser will perform substitutions before interpreting
+the expression. This is not actually the desired behavior in most cases, and may
+impact functionality in some edge cases. In addition, this can reduce
+performance.
+
+See "Performance Considerations" in the [Tcl docs for `expr`](https://www.tcl.tk/man/tcl/TclCmd/expr.html).
```

### Comparing `tclint-0.2.2/pyproject.toml` & `tclint-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     {name = "Noah Moroze", email = "me@noahmoroze.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "ply==3.11",
     "schema==0.7.5",
-    "tomli~=2.0.1; python_version < '3.11'"
+    "tomli~=2.0.1; python_version < '3.11'",
+    "pathspec==0.11.2"
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "flake8",
     "pytest",
```

### Comparing `tclint-0.2.2/src/tclint/checks.py` & `tclint-0.2.3/src/tclint/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 
 from tclint.commands import get_commands
 from tclint.violations import Rule, Violation
 
-from tclint.syntax_tree import Visitor, Script, List, ParenExpression
+from tclint.syntax_tree import Visitor, Script, List, ParenExpression, BracedExpression
 
 
 class IndentLevelChecker(Visitor):
     """Checks that each line is indented at the correct level.
 
     Reports 'indent' violations.
     """
@@ -469,15 +469,15 @@
                     # TODO: consider flagging violation here? this is probably
                     # not a necessary "\". could also be worth checking
                     # indentation of a lonely "\", if we allow them
                     continue
                 if whitespace_count != 1 or line[-2] == "\t":
                     violations.append(
                         Violation(
-                            Rule.BACKSLACH_SPACING,
+                            Rule.BACKSLASH_SPACING,
                             "expected 1 space between line contents and backslash",
                             (lineno, len(line)),
                         )
                     )
 
         return violations
 
@@ -724,17 +724,43 @@
                     Rule.SPACES_IN_BRACES,
                     message,
                     last.end_pos,
                 )
             )
 
 
+class UnbracedExprChecker(Visitor):
+    def check(self, _, tree, __):
+        self._violations = []
+        tree.accept(self, recurse=True)
+        return self._violations
+
+    def visit_command(self, command):
+        if command.routine != "expr":
+            return
+
+        if len(command.args) == 1 and isinstance(command.args[0], BracedExpression):
+            return
+
+        for child in command.args:
+            if child.contents is None:
+                self._violations.append(
+                    Violation(
+                        Rule.UNBRACED_EXPR,
+                        "expression with substitutions should be enclosed by braces",
+                        command.args[0].pos,
+                    )
+                )
+                return
+
+
 def get_checkers():
     return (
         IndentLevelChecker(),
         SpacingChecker(),
         LineChecker(),
         RedefinedBuiltinChecker(),
         BlankLineChecker(),
         BackslashNewlineChecker(),
         SpacesInBracesChecker(),
+        UnbracedExprChecker(),
     )
```

### Comparing `tclint-0.2.2/src/tclint/commands/__init__.py` & `tclint-0.2.3/src/tclint/commands/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from importlib.metadata import entry_points
 from typing import List, Dict
 
 from tclint.commands import builtin as _builtin
+from tclint.commands.plugins import PluginManager
 
 # import to expose in package
 from tclint.commands.utils import CommandArgError
 
 __all__ = ["CommandArgError", "validate_command_plugins", "get_commands"]
 
 
@@ -18,59 +19,25 @@
         except KeyError:
             return []
     else:
         return entry_points(group=group)
 
 
 def validate_command_plugins(plugins: List[str]) -> List[str]:
-    plugins_set = set(plugins)
-    installed_plugins = _get_entry_points("tclint.plugins")
+    valid_plugins = []
+    for plugin in set(plugins):
+        if PluginManager.load(plugin) is not None:
+            valid_plugins.append(plugin)
 
-    plugins_found = set()
-    for plugin in installed_plugins:
-        if plugin.name not in plugins_set:
-            continue
-
-        try:
-            module = plugin.load()
-        except Exception:
-            print(
-                f"Warning: skipping plugin {plugin.name} due to an error in the plugin"
-            )
-            continue
-
-        if not hasattr(module, "commands"):
-            print(
-                f"Warning: skipping plugin {plugin.name} since it does not define"
-                " commands"
-            )
-            continue
-
-        plugins_found.add(plugin.name)
-
-    plugins_diff = plugins_set.difference(plugins_found)
-    if plugins_diff:
-        plugins_str = ", ".join(plugins_diff)
-        print(f"Warning: following plugins could not be found: {plugins_str}")
-
-    return list(plugins_found)
+    return valid_plugins
 
 
 def get_commands(plugins: List[str]) -> Dict:
-    plugins_to_find = set(plugins)
-    installed_plugins = _get_entry_points("tclint.plugins")
-
     commands = {}
     commands.update(_builtin.commands)
 
-    for plugin in installed_plugins:
-        try:
-            plugins_to_find.remove(plugin.name)
-        except KeyError:
-            continue
-
-        module = plugin.load()
-        plugin_commands = getattr(module, "commands")
-
-        commands.update(plugin_commands)
+    for plugin in set(plugins):
+        plugin_commands = PluginManager.load(plugin)
+        if plugin_commands is not None:
+            commands.update(plugin_commands)
 
     return commands
```

### Comparing `tclint-0.2.2/src/tclint/commands/builtin.py` & `tclint-0.2.3/src/tclint/commands/builtin.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/src/tclint/commands/utils.py` & `tclint-0.2.3/src/tclint/commands/utils.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/src/tclint/comments.py` & `tclint-0.2.3/src/tclint/comments.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/src/tclint/config.py` & `tclint-0.2.3/src/tclint/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return [v.strip() for v in s.split(",")]
     return s
 
 
 _VALIDATORS = {
     # note: it's ok if paths don't exist - allows for generic
     # configurations with directories like .git/ excluded
-    "exclude": And(Use(_str2list), [Use(pathlib.Path)]),
+    "exclude": Use(_str2list),
     "ignore": And(
         Use(_str2list),
         [
             Or(
                 Use(
                     Rule,
                     error="invalid rule ID provided for 'ignore'",
```

### Comparing `tclint-0.2.2/src/tclint/lexer.py` & `tclint-0.2.3/src/tclint/lexer.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/src/tclint/parser.py` & `tclint-0.2.3/src/tclint/parser.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/src/tclint/syntax_tree.py` & `tclint-0.2.3/src/tclint/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/src/tclint/tclint.py` & `tclint-0.2.3/src/tclint/tclint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Main CLI entry point."""
 
 import argparse
 import codecs
 import os
 import pathlib
+import re
 import sys
 from typing import List, Optional
 
+import pathspec
+
 from tclint.config import get_config, setup_config_cli_args, Config, ConfigError
 from tclint.parser import Parser, TclSyntaxError
 from tclint.checks import get_checkers
 from tclint.violations import Violation, Rule
 from tclint.comments import CommentVisitor
 from tclint import utils
 
@@ -23,40 +26,49 @@
 EXIT_OK = 0
 EXIT_LINT_VIOLATIONS = 1
 EXIT_SYNTAX_ERROR = 2
 EXIT_INPUT_ERROR = 4
 
 
 def resolve_sources(
-    paths: List[pathlib.Path], exclude: Optional[List[pathlib.Path]] = None
+    paths: List[pathlib.Path], exclude_patterns: List[str], exclude_root: pathlib.Path
 ) -> List[Optional[pathlib.Path]]:
     """Resolves paths passed via CLI to a list of filepaths to lint.
 
     `paths` is a list of paths that may be files or directories. Files are
     returned verbatim if they exist, and directories are recursively searched
-    for files that have the extension .tcl, .xdc, or .sdc. Paths that match or
-    are underneath a path provided in `exclude` are ignored.
+    for files that have the extension .tcl, .xdc, or .sdc. Paths that match a
+    pattern in `exclude_patterns` are ignored (based on gitignore pattern
+    format, see https://git-scm.com/docs/gitignore#_pattern_format).
 
     Raises FileNotFoundError if a supplied path does not exist.
     """
     # Extensions that may indicate tcl files
     # TODO: make configurable
     EXTENSIONS = [".tcl", ".xdc", ".sdc"]
 
-    if exclude is None:
-        exclude = []
-    exclude = [path.resolve() for path in exclude]
+    exclude_root = exclude_root.resolve()
+    exclude_patterns = [
+        re.sub(r"^\s*#", r"\#", pattern) for pattern in exclude_patterns
+    ]
+    exclude_spec = pathspec.PathSpec.from_lines("gitwildmatch", exclude_patterns)
 
     def is_excluded(path):
-        resolved_path = path.resolve()
-        for exclude_path in exclude:
-            # if the current path is under an excluded path it should be ignored
-            if utils.is_relative_to(resolved_path, exclude_path):
-                return True
+        abspath = path.resolve()
+        try:
+            relpath = os.path.relpath(abspath, start=exclude_root)
+        except ValueError:
+            print(
+                "Warning: processing files on different drive from where tclint was"
+                " run, 'exclude' config may not behave as expected"
+            )
+            relpath = abspath
 
+        if exclude_spec.match_file(relpath):
+            return True
         return False
 
     sources: List[Optional[pathlib.Path]] = []
 
     for path in paths:
         if str(path) == "-":
             sources.append(None)
@@ -167,27 +179,38 @@
         "-c",
         "--config",
         help="path to config file",
         type=pathlib.Path,
         default=None,
         metavar="<path>",
     )
+    parser.add_argument(
+        "--show-categories",
+        help="print category tag for each violation",
+        action="store_true",
+    )
     setup_config_cli_args(parser)
     args = parser.parse_args()
 
     try:
         config = get_config(args.config)
     except ConfigError as e:
         print(f"Invalid config file: {e}")
         return EXIT_INPUT_ERROR
 
     config.apply_cli_args(args)
 
     try:
-        sources = resolve_sources(args.source, exclude=config.exclude)
+        # TODO: we should eventually allow tclint to find a config by walking up
+        # directories, at which point exclude_root should be the parent dir of
+        # the config file, unless -c is used (eslint rules)
+        exclude_root = pathlib.Path.cwd()
+        sources = resolve_sources(
+            args.source, exclude_patterns=config.exclude, exclude_root=exclude_root
+        )
     except FileNotFoundError as e:
         print(f"Invalid path provided: {e}")
         return EXIT_INPUT_ERROR
 
     retcode = EXIT_OK
 
     for path in sources:
@@ -204,15 +227,15 @@
         except TclSyntaxError as e:
             line, col = e.pos
             print(f"{out_prefix}:{line}:{col}: syntax error: {e}")
             retcode |= EXIT_SYNTAX_ERROR
             continue
 
         for violation in sorted(violations):
-            print(f"{out_prefix}:{violation}")
+            print(f"{out_prefix}:{violation.str(show_category=args.show_categories)}")
 
         if len(violations) > 0:
             retcode |= EXIT_LINT_VIOLATIONS
 
     return retcode
```

### Comparing `tclint-0.2.2/src/tclint.egg-info/PKG-INFO` & `tclint-0.2.3/src/tclint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tclint
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI utility for linting and analyzing Tcl code.
 Author-email: Noah Moroze <me@noahmoroze.com>
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply==3.11
 Requires-Dist: schema==0.7.5
 Requires-Dist: tomli~=2.0.1; python_version < "3.11"
+Requires-Dist: pathspec==0.11.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 
 # tclint &nbsp; [![CI](https://github.com/nmoroze/tclint/actions/workflows/ci.yml/badge.svg)](https://github.com/nmoroze/tclint/actions/workflows/ci.yml)
```

### Comparing `tclint-0.2.2/src/tclint.egg-info/SOURCES.txt` & `tclint-0.2.3/src/tclint.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/tclint.egg-info/SOURCES.txt
 src/tclint.egg-info/dependency_links.txt
 src/tclint.egg-info/entry_points.txt
 src/tclint.egg-info/requires.txt
 src/tclint.egg-info/top_level.txt
 src/tclint/commands/__init__.py
 src/tclint/commands/builtin.py
+src/tclint/commands/plugins.py
 src/tclint/commands/utils.py
 tests/test_config.py
 tests/test_lint.py
 tests/test_parser.py
 tests/test_tclint.py
 tests/data/backslash-spacing.tcl
 tests/data/backslash-spacing.txt
```

### Comparing `tclint-0.2.2/tests/data/blank-lines.txt` & `tclint-0.2.3/tests/data/blank-lines.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/tests/data/dirty.txt` & `tclint-0.2.3/tests/data/dirty.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 data/dirty.tcl:1:14: expected 1 space between words, got 2 [spacing]
 data/dirty.tcl:2:1: expected indent of 4 spaces, got 0 [indent]
 data/dirty.tcl:3:1: expected indent of 8 spaces, got 0 [indent]
 data/dirty.tcl:4:1: expected indent of 4 spaces, got 0 [indent]
 data/dirty.tcl:4:2: expected 1 space between words, got 3 [spacing]
 data/dirty.tcl:6:1: expected indent of 4 spaces, got 0 [indent]
+data/dirty.tcl:6:17: expression with substitutions should be enclosed by braces [unbraced-expr]
 data/dirty.tcl:7:13: expected 1 space between words, got 3 [spacing]
 data/dirty.tcl:9:13: expected 1 space between words, got 5 [spacing]
```

### Comparing `tclint-0.2.2/tests/data/expr-format.txt` & `tclint-0.2.3/tests/data/expr-format.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/tests/data/indent.txt` & `tclint-0.2.3/tests/data/indent.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/tests/data/indent_lists.tcl` & `tclint-0.2.3/tests/data/indent_lists.tcl`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/tests/data/spaces-in-braces.txt` & `tclint-0.2.3/tests/data/spaces-in-braces.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/tests/data/tclint.toml` & `tclint-0.2.3/tests/data/tclint.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # paths to exclude when searching directories. defaults to empty list.
-exclude = ["ignore_me/", "ignore.tcl"]
+exclude = ["ignore_me/", "ignore*.tcl", "/ignore_from_here"]
 # lint violations to ignore. defaults to empty list.
 # can also supply an inline table with a path and a list of violations to ignore under that path.
 ignore = [
     "spacing",
     { path = "files_with_bad_indent/", rules = ["indent"] }
 ]
```

### Comparing `tclint-0.2.2/tests/test_config.py` & `tclint-0.2.3/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def test_example_config():
     config_path = MY_DIR / "data" / "tclint.toml"
     config = get_config(config_path)
 
     global_ = config.get_for_path(pathlib.Path())
 
-    assert global_.exclude == list(map(pathlib.Path, ["ignore_me/", "ignore.tcl"]))
+    assert global_.exclude == ["ignore_me/", "ignore*.tcl", "/ignore_from_here"]
     assert global_.ignore == [
         Rule("spacing"),
         {"path": pathlib.Path("files_with_bad_indent/"), "rules": [Rule("indent")]},
     ]
 
     assert global_.style_indent == 2
     assert global_.style_line_length == 100
```

### Comparing `tclint-0.2.2/tests/test_lint.py` & `tclint-0.2.3/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.2/tests/test_parser.py` & `tclint-0.2.3/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,60 +260,51 @@
             ),
             Script(Command(BareWord("incr"), BareWord("i"))),
             Script(
                 Command(
                     BareWord("if"),
                     BracedExpression(
                         BinaryOp(
-                            CommandSub(
-                                Command(
-                                    BareWord("expr"),
-                                    VarSub("i"),
-                                    BareWord("%"),
-                                    BareWord("15"),
-                                )
+                            VarSub("i"),
+                            BareWord("%"),
+                            BinaryOp(
+                                BareWord("15"),
+                                BareWord("=="),
+                                BareWord("0"),
                             ),
-                            BareWord("=="),
-                            BareWord("0"),
                         ),
                     ),
                     Script(
                         Command(BareWord("puts"), QuotedWord(BareWord("FizzBuzz"))),
                     ),
                     BareWord("elseif"),
                     BracedExpression(
                         BinaryOp(
-                            CommandSub(
-                                Command(
-                                    BareWord("expr"),
-                                    VarSub("i"),
-                                    BareWord("%"),
-                                    BareWord("3"),
-                                )
+                            VarSub("i"),
+                            BareWord("%"),
+                            BinaryOp(
+                                BareWord("3"),
+                                BareWord("=="),
+                                BareWord("0"),
                             ),
-                            BareWord("=="),
-                            BareWord("0"),
                         ),
                     ),
                     Script(
                         Command(BareWord("puts"), QuotedWord(BareWord("Fizz"))),
                     ),
                     BareWord("elseif"),
                     BracedExpression(
                         BinaryOp(
-                            CommandSub(
-                                Command(
-                                    BareWord("expr"),
-                                    VarSub("i"),
-                                    BareWord("%"),
-                                    BareWord("5"),
-                                )
+                            VarSub("i"),
+                            BareWord("%"),
+                            BinaryOp(
+                                BareWord("5"),
+                                BareWord("=="),
+                                BareWord("0"),
                             ),
-                            BareWord("=="),
-                            BareWord("0"),
                         ),
                     ),
                     Script(
                         Command(BareWord("puts"), QuotedWord(BareWord("Buzz"))),
                     ),
                     BareWord("else"),
                     Script(
```

