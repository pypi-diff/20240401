# Comparing `tmp/ddsketch-2.0.4.tar.gz` & `tmp/ddsketch-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddsketch-2.0.4.tar", last modified: Thu Jul 21 18:16:12 2022, max compression
+gzip compressed data, was "ddsketch-3.0.1.tar", last modified: Mon Apr  1 13:11:01 2024, max compression
```

## Comparing `ddsketch-2.0.4.tar` & `ddsketch-3.0.1.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.509734 ddsketch-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.497734 ddsketch-2.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-07-21 18:16:00.000000 ddsketch-2.0.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-21 18:16:00.000000 ddsketch-2.0.4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.497734 ddsketch-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-07-21 18:16:00.000000 ddsketch-2.0.4/.github/workflows/build_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-07-21 18:16:00.000000 ddsketch-2.0.4/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-07-21 18:16:00.000000 ddsketch-2.0.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-07-21 18:16:00.000000 ddsketch-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-21 18:16:00.000000 ddsketch-2.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-07-21 18:16:00.000000 ddsketch-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-07-21 18:16:00.000000 ddsketch-2.0.4/LICENSE-3rdparty.csv
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-07-21 18:16:00.000000 ddsketch-2.0.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     5300 2022-07-21 18:16:12.509734 ddsketch-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-07-21 18:16:00.000000 ddsketch-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.501734 ddsketch-2.0.4/ddsketch/
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-21 18:16:12.000000 ddsketch-2.0.4/ddsketch/__version.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    11444 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/ddsketch.py
--rw-r--r--   0 runner    (1001) docker     (121)     7759 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.501734 ddsketch-2.0.4/ddsketch/pb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/pb/ddsketch.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3580 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/pb/ddsketch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10087 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/pb/ddsketch_pre319_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3315 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/pb/proto.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17515 2022-07-21 18:16:00.000000 ddsketch-2.0.4/ddsketch/store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.501734 ddsketch-2.0.4/ddsketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5300 2022-07-21 18:16:12.000000 ddsketch-2.0.4/ddsketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-07-21 18:16:12.000000 ddsketch-2.0.4/ddsketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 18:16:12.000000 ddsketch-2.0.4/ddsketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-07-21 18:16:12.000000 ddsketch-2.0.4/ddsketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-21 18:16:12.000000 ddsketch-2.0.4/ddsketch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-07-21 18:16:00.000000 ddsketch-2.0.4/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-07-21 18:16:00.000000 ddsketch-2.0.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-07-21 18:16:00.000000 ddsketch-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.501734 ddsketch-2.0.4/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.509734 ddsketch-2.0.4/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/ddsketch-api-a84ffc0875bbacd6.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/extend-range-06474632c8235187.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/proto4-e8646610178bef59.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/protobuf-min-f6af9a2d5d96f53c.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/py2-c963608396db7258.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/py310-ac5baa9b0b69008a.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/remove-custom-exceptions-e2bc67a72250269d.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/remove-numpy-25fedcd9be9d6d80.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/tests-wheel-bf71b228c86a9ced.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/toplevelapi-6c04f2ca35a49d4b.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/typing-25579ab88323a332.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-07-21 18:16:00.000000 ddsketch-2.0.4/releasenotes/notes/version-b2a276df190a703a.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-07-21 18:16:00.000000 ddsketch-2.0.4/riotfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.509734 ddsketch-2.0.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      918 2022-07-21 18:16:00.000000 ddsketch-2.0.4/scripts/check-releasenotes
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-07-21 18:16:12.509734 ddsketch-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-07-21 18:16:00.000000 ddsketch-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:12.509734 ddsketch-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 18:16:00.000000 ddsketch-2.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8541 2022-07-21 18:16:00.000000 ddsketch-2.0.4/tests/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     8455 2022-07-21 18:16:00.000000 ddsketch-2.0.4/tests/test_ddsketch.py
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-07-21 18:16:00.000000 ddsketch-2.0.4/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-07-21 18:16:00.000000 ddsketch-2.0.4/tests/test_proto.py
--rw-r--r--   0 runner    (1001) docker     (121)    10133 2022-07-21 18:16:00.000000 ddsketch-2.0.4/tests/test_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.615191 ddsketch-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.607190 ddsketch-3.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 13:10:58.000000 ddsketch-3.0.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-01 13:10:58.000000 ddsketch-3.0.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.607190 ddsketch-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-01 13:10:58.000000 ddsketch-3.0.1/.github/workflows/build_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-01 13:10:58.000000 ddsketch-3.0.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-01 13:10:58.000000 ddsketch-3.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-01 13:10:58.000000 ddsketch-3.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 13:10:58.000000 ddsketch-3.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-01 13:10:58.000000 ddsketch-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-01 13:10:58.000000 ddsketch-3.0.1/LICENSE-3rdparty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 13:10:58.000000 ddsketch-3.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-01 13:11:01.615191 ddsketch-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-01 13:10:58.000000 ddsketch-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.611190 ddsketch-3.0.1/ddsketch/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 13:11:01.000000 ddsketch-3.0.1/ddsketch/__version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/ddsketch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.611190 ddsketch-3.0.1/ddsketch/pb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/pb/ddsketch.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/pb/ddsketch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/pb/ddsketch_pre319_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/pb/proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17543 2024-04-01 13:10:58.000000 ddsketch-3.0.1/ddsketch/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.611190 ddsketch-3.0.1/ddsketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-01 13:11:01.000000 ddsketch-3.0.1/ddsketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-01 13:11:01.000000 ddsketch-3.0.1/ddsketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:11:01.000000 ddsketch-3.0.1/ddsketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 13:11:01.000000 ddsketch-3.0.1/ddsketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 13:11:01.000000 ddsketch-3.0.1/ddsketch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-01 13:10:58.000000 ddsketch-3.0.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-01 13:10:58.000000 ddsketch-3.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-01 13:10:58.000000 ddsketch-3.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.611190 ddsketch-3.0.1/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.615191 ddsketch-3.0.1/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/ddsketch-api-a84ffc0875bbacd6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/extend-range-06474632c8235187.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/oldpy-db6189c9b26e10f7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/pbopt-ec6525c1948d782f.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/proto4-e8646610178bef59.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/protobuf-min-f6af9a2d5d96f53c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/py2-c963608396db7258.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/py310-ac5baa9b0b69008a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/remove-custom-exceptions-e2bc67a72250269d.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/remove-numpy-25fedcd9be9d6d80.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/tests-wheel-bf71b228c86a9ced.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/toplevelapi-6c04f2ca35a49d4b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/typing-25579ab88323a332.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 13:10:58.000000 ddsketch-3.0.1/releasenotes/notes/version-b2a276df190a703a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-01 13:10:58.000000 ddsketch-3.0.1/riotfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.615191 ddsketch-3.0.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-01 13:10:58.000000 ddsketch-3.0.1/scripts/check-releasenotes
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 13:11:01.615191 ddsketch-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 13:10:58.000000 ddsketch-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:11:01.615191 ddsketch-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:10:58.000000 ddsketch-3.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-01 13:10:58.000000 ddsketch-3.0.1/tests/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-01 13:10:58.000000 ddsketch-3.0.1/tests/test_ddsketch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-01 13:10:58.000000 ddsketch-3.0.1/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-01 13:10:58.000000 ddsketch-3.0.1/tests/test_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-04-01 13:10:58.000000 ddsketch-3.0.1/tests/test_store.py
```

### Comparing `ddsketch-2.0.4/.github/workflows/build_deploy.yml` & `ddsketch-3.0.1/.github/workflows/build_deploy.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   release:
     types:
       - published
 
 jobs:
   build_wheel:
     name: Build wheels
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
 
     steps:
       - uses: actions/checkout@v2
         # Include all history and tags
         with:
           fetch-depth: 0
```

### Comparing `ddsketch-2.0.4/.github/workflows/changelog.yml` & `ddsketch-3.0.1/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/.github/workflows/test.yml` & `ddsketch-3.0.1/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,37 @@
     branches:
       - master
   pull_request:
 jobs:
   check:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v5
         with:
-          python-version: '3.9'
-      - uses: actions/checkout@v2
+          python-version: '3.12'
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - run: pip install riot==0.9.0
+      - run: pip install riot==0.19.0
       - run: riot -v run check_fmt
       - run: riot -v run -s mypy
       - run: riot -v run -s flake8
 
   test:
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest]
-        python-version: ["2.7", "3.6", "3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
     runs-on: ${{ matrix.os }}
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: install riot
         # Note that pip3 has to be used since the system pip when running
         # under the 2.7 instance will be Python 2 pip.
         # (riot is not Python 2 compatible)
-        run: pip3 install riot==0.9.0
+        run: pip3 install riot==0.19.0
       - run: |
           riot run -p ${{ matrix.python-version}} test
```

### Comparing `ddsketch-2.0.4/LICENSE` & `ddsketch-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/PKG-INFO` & `ddsketch-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ddsketch
-Version: 2.0.4
+Version: 3.0.1
 Summary: Distributed quantile sketches
 Home-page: http://github.com/datadog/sketches-py
 Author: Jee Rim, Charles-Philippe Masson, Homin Lee
 Author-email: jee.rim@datadoghq.com, charles.masson@datadoghq.com, homin@datadoghq.com
 License: UNKNOWN
 Download-URL: https://github.com/DataDog/sketches-py/archive/v1.0.tar.gz
 Keywords: ddsketch,quantile,sketch
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=2.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: serialization
 License-File: LICENSE
 License-File: LICENSE-3rdparty.csv
 License-File: NOTICE
 
 # ddsketch
 
 This repo contains the Python implementation of the distributed quantile sketch
```

### Comparing `ddsketch-2.0.4/README.md` & `ddsketch-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/ddsketch/__init__.py` & `ddsketch-3.0.1/ddsketch/__init__.py`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/ddsketch/ddsketch.py` & `ddsketch-3.0.1/ddsketch/ddsketch.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 from .mapping import LogarithmicMapping
 from .store import CollapsingHighestDenseStore
 from .store import CollapsingLowestDenseStore
 from .store import DenseStore
 
 
 if typing.TYPE_CHECKING:
-    from typing import Optional
+    from typing import Optional  # noqa: F401
 
-    from .mapping import KeyMapping
-    from .store import Store
+    from .mapping import KeyMapping  # noqa: F401
+    from .store import Store  # noqa: F401
 
 
 DEFAULT_REL_ACC = 0.01  # "alpha" in the paper
 DEFAULT_BIN_LIMIT = 2048
 
 
 class BaseDDSketch(object):
```

### Comparing `ddsketch-2.0.4/ddsketch/mapping.py` & `ddsketch-3.0.1/ddsketch/mapping.py`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/ddsketch/pb/ddsketch.proto` & `ddsketch-3.0.1/ddsketch/pb/ddsketch.proto`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/ddsketch/pb/ddsketch_pb2.py` & `ddsketch-3.0.1/ddsketch/pb/ddsketch_pb2.py`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/ddsketch/pb/ddsketch_pre319_pb2.py` & `ddsketch-3.0.1/ddsketch/pb/ddsketch_pre319_pb2.py`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/ddsketch/pb/proto.py` & `ddsketch-3.0.1/ddsketch/pb/proto.py`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/ddsketch/store.py` & `ddsketch-3.0.1/ddsketch/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 import abc
 import math
 import typing
 
 
 if typing.TYPE_CHECKING:
-    from typing import List
-    from typing import Optional
+    from typing import List  # noqa: F401
+    from typing import Optional  # noqa: F401
 
 import six
 
 
 CHUNK_SIZE = 128
```

### Comparing `ddsketch-2.0.4/ddsketch.egg-info/PKG-INFO` & `ddsketch-3.0.1/ddsketch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ddsketch
-Version: 2.0.4
+Version: 3.0.1
 Summary: Distributed quantile sketches
 Home-page: http://github.com/datadog/sketches-py
 Author: Jee Rim, Charles-Philippe Masson, Homin Lee
 Author-email: jee.rim@datadoghq.com, charles.masson@datadoghq.com, homin@datadoghq.com
 License: UNKNOWN
 Download-URL: https://github.com/DataDog/sketches-py/archive/v1.0.tar.gz
 Keywords: ddsketch,quantile,sketch
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=2.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: serialization
 License-File: LICENSE
 License-File: LICENSE-3rdparty.csv
 License-File: NOTICE
 
 # ddsketch
 
 This repo contains the Python implementation of the distributed quantile sketch
```

### Comparing `ddsketch-2.0.4/ddsketch.egg-info/SOURCES.txt` & `ddsketch-3.0.1/ddsketch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 ddsketch/pb/ddsketch.proto
 ddsketch/pb/ddsketch_pb2.py
 ddsketch/pb/ddsketch_pre319_pb2.py
 ddsketch/pb/proto.py
 releasenotes/config.yaml
 releasenotes/notes/ddsketch-api-a84ffc0875bbacd6.yaml
 releasenotes/notes/extend-range-06474632c8235187.yaml
+releasenotes/notes/oldpy-db6189c9b26e10f7.yaml
+releasenotes/notes/pbopt-ec6525c1948d782f.yaml
 releasenotes/notes/proto4-e8646610178bef59.yaml
 releasenotes/notes/protobuf-min-f6af9a2d5d96f53c.yaml
 releasenotes/notes/py2-c963608396db7258.yaml
 releasenotes/notes/py310-ac5baa9b0b69008a.yaml
 releasenotes/notes/remove-custom-exceptions-e2bc67a72250269d.yaml
 releasenotes/notes/remove-numpy-25fedcd9be9d6d80.yaml
 releasenotes/notes/tests-wheel-bf71b228c86a9ced.yaml
```

### Comparing `ddsketch-2.0.4/riotfile.py` & `ddsketch-3.0.1/riotfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,33 +10,23 @@
             command="pytest {cmdargs}",
             pkgs={
                 "pytest": latest,
                 "numpy": latest,
             },
             venvs=[
                 Venv(
-                    pys=["2.7", "3.6"],
-                    pkgs={
-                        "protobuf": [
-                            "==3.0.0",
-                            "<3.19",
-                            "!=4.21.0",
-                        ],  # not latest due to https://github.com/protocolbuffers/protobuf/issues/10053
-                    },
-                ),
-                Venv(
                     pys=["3.7", "3.8", "3.9"],
                     pkgs={
-                        "protobuf": ["==3.0.0", "<3.19", latest],
+                        "protobuf": ["==3.0.0", latest],
                     },
                 ),
                 Venv(
-                    pys=["3.10"],
+                    pys=["3.10", "3.11", "3.12"],
                     pkgs={
-                        "protobuf": ["==3.8.0", "<3.19.0", latest],
+                        "protobuf": ["==3.8.0", latest],
                     },
                 ),
             ],
         ),
         Venv(
             pkgs={
                 "reno": latest,
@@ -52,15 +42,14 @@
             name="flake8",
             command="flake8 {cmdargs}",
             pkgs={
                 "flake8": latest,
                 "flake8-blind-except": latest,
                 "flake8-builtins": latest,
                 "flake8-docstrings": latest,
-                "flake8-logging-format": latest,
                 "flake8-rst-docstrings": latest,
                 # needed for some features from flake8-rst-docstrings
                 "pygments": latest,
             },
         ),
         Venv(
             pkgs={
```

### Comparing `ddsketch-2.0.4/scripts/check-releasenotes` & `ddsketch-3.0.1/scripts/check-releasenotes`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/tests/datasets.py` & `ddsketch-3.0.1/tests/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,27 +214,25 @@
                 initial_item += initial_skip
                 i += 1
             else:
                 initial_item += 1
 
 
 class Constant(Dataset):
-
     constant = 42.0
 
     @property
     def name(self):
         return "constant"
 
     def populate(self):
         return [self.constant] * self.size
 
 
 class Exponential(Dataset):
-
     scale = 0.01
 
     @classmethod
     def from_params(cls, scale, n):
         cls.scale = scale
         return cls(n)
 
@@ -243,15 +241,14 @@
         return "exponential"
 
     def populate(self):
         return np.random.exponential(scale=self.scale, size=self.size)
 
 
 class Lognormal(Dataset):
-
     scale = 100.0
 
     @classmethod
     def from_params(cls, scale, n):
         cls.scale = scale
         return cls(n)
 
@@ -260,15 +257,14 @@
         return "lognormal"
 
     def populate(self):
         return np.random.lognormal(size=self.size) / self.scale
 
 
 class Normal(Dataset):
-
     loc = 37.4
     scale = 1.0
 
     @classmethod
     def from_params(cls, loc, scale, n):
         cls.loc = loc
         cls.scale = scale
@@ -279,15 +275,14 @@
         return "normal"
 
     def populate(self):
         return np.random.normal(loc=self.loc, scale=self.scale, size=self.size)
 
 
 class Laplace(Dataset):
-
     loc = 11278.0
     scale = 100.0
 
     @classmethod
     def from_params(cls, loc, scale, n):
         cls.loc = loc
         cls.scale = scale
@@ -298,15 +293,14 @@
         return "laplace"
 
     def populate(self):
         return np.random.laplace(loc=self.loc, scale=self.scale, size=self.size)
 
 
 class Bimodal(Dataset):
-
     right_loc = 17.3
     left_loc = -2.0
     left_std = 3.0
 
     @property
     def name(self):
         return "bimodal"
@@ -318,15 +312,14 @@
         if np.random.random() > 0.5:
             yield np.random.laplace(self.right_loc)
         else:
             yield np.random.normal(self.left_loc, self.left_std)
 
 
 class Mixed(Dataset):
-
     mean = 0.0
     sigma = 0.25
     scale_factor = 0.1
 
     loc = 10.0
     scale = 0.5
 
@@ -347,15 +340,14 @@
         if np.random.random() < self.ratio:
             yield self.scale_factor * np.random.lognormal(self.mean, self.sigma)
         else:
             yield np.random.normal(self.loc, self.scale)
 
 
 class Trimodal(Dataset):
-
     right_loc = 17.3
     left_loc = 5.0
     left_std = 0.5
     exp_scale = 0.01
 
     @property
     def name(self):
@@ -370,15 +362,14 @@
         elif np.random.random() > 1.0 / 3.0:
             yield np.random.normal(self.left_loc, self.left_std)
         else:
             yield np.random.exponential(scale=self.exp_scale)
 
 
 class Integers(Dataset):
-
     loc = 4.3
     scale = 5.0
 
     @classmethod
     def from_params(cls, loc, scale, n):
         cls.loc = loc
         cls.scale = scale
```

### Comparing `ddsketch-2.0.4/tests/test_ddsketch.py` & `ddsketch-3.0.1/tests/test_ddsketch.py`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/tests/test_mapping.py` & `ddsketch-3.0.1/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `ddsketch-2.0.4/tests/test_proto.py` & `ddsketch-3.0.1/tests/test_proto.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         rel_accs = [1e-1, 1e-2, 1e-8]
         for rel_acc in rel_accs:
             for offset in self.offsets:
                 mapping = self.mapping(rel_acc, offset)
                 round_trip_mapping = KeyMappingProto.from_proto(
                     KeyMappingProto.to_proto(mapping)
                 )
-                assert type(mapping) == type(round_trip_mapping)
+                assert type(mapping) == type(round_trip_mapping)  # noqa: E721
                 assert mapping.relative_accuracy == pytest.approx(
                     round_trip_mapping.relative_accuracy
                 )
                 assert mapping.value(0) == pytest.approx(round_trip_mapping.value(0))
 
 
 class TestLogarithmicMapping(BaseTestKeyMappingProto, TestCase):
```

### Comparing `ddsketch-2.0.4/tests/test_store.py` & `ddsketch-3.0.1/tests/test_store.py`

 * *Files identical despite different names*

