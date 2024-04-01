# Comparing `tmp/allure-robotframework-2.9.44.tar.gz` & `tmp/allure-robotframework-2.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allure-robotframework-2.9.44.tar", last modified: Wed Sep 29 20:24:42 2021, max compression
+gzip compressed data, was "allure-robotframework-2.9.45.tar", last modified: Fri Oct 15 08:22:36 2021, max compression
```

## Comparing `allure-robotframework-2.9.44.tar` & `allure-robotframework-2.9.45.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/allure_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-09-29 20:24:41.000000 allure-robotframework-2.9.44/allure_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-09-29 20:24:41.000000 allure-robotframework-2.9.44/allure_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 20:24:41.000000 allure-robotframework-2.9.44/allure_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-09-29 20:24:41.000000 allure-robotframework-2.9.44/allure_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-09-29 20:24:41.000000 allure-robotframework-2.9.44/allure_robotframework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/attach/
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/attach/data_attach.rst
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/attach/file_attach.rst
--rw-r--r--   0 runner    (1001) docker     (121)      394 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/attach/foreign_library.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/attach/foreign_library_attach.rst
--rw-r--r--   0 runner    (1001) docker     (121)      685 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/attach/foreign_library_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/description/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/description/testcase_description.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/fixture/
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/fixture/testcase_fixture.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/label/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/label/__init__.rst
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/label/labels_library.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/label/testcase_bdd_label.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/label/testcase_custom_labels.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/link/
--rw-r--r--   0 runner    (1001) docker     (121)      468 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/link/dynamic_link.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/link/link.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/status/
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/status/status.rst
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/status/status_library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/step/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/step/builtin_step.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/step/outside_step.rst
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/step/outside_step_library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/tag/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/tag/tag.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/examples/testplan/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/examples/testplan/testplan.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.081856 allure-robotframework-2.9.44/src/library/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/library/allure_library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/src/listener/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/listener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10936 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/listener/allure_listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/listener/allure_testplan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/listener/robot_listener.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/listener/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/src/listener/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/attach/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/attach/data_attach.robot
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/attach/file_attach.robot
--rw-r--r--   0 runner    (1001) docker     (121)      522 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/attach/foreign_library_attach.robot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/description/
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/description/testcase_description.robot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/fixture/suite_fixture.robot
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/fixture/testcase_fixture.robot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/label/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/label/testcase_bdd_label.robot
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/label/testcase_custom_labels.robot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/link/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/link/dynamic_link.robot
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/link/link.robot
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/link/suite_link.robot
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/run_robot_library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/status/
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/status/status.robot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/step/
--rw-r--r--   0 runner    (1001) docker     (121)      597 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/step/builtin_step.robot
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/step/outside_step.robot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/tag/
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/tag/tag.robot
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/test_allure_library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:42.085856 allure-robotframework-2.9.44/test/testplan/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/test/testplan/testplan.robot
--rw-r--r--   0 runner    (1001) docker     (121)      806 2021-09-29 20:24:05.000000 allure-robotframework-2.9.44/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.964933 allure-robotframework-2.9.45/allure_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-10-15 08:22:36.000000 allure-robotframework-2.9.45/allure_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-10-15 08:22:36.000000 allure-robotframework-2.9.45/allure_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 08:22:36.000000 allure-robotframework-2.9.45/allure_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-15 08:22:36.000000 allure-robotframework-2.9.45/allure_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-10-15 08:22:36.000000 allure-robotframework-2.9.45/allure_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.960933 allure-robotframework-2.9.45/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.964933 allure-robotframework-2.9.45/examples/attach/
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/attach/data_attach.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/attach/file_attach.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/attach/foreign_library.py
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/attach/foreign_library_attach.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/attach/foreign_library_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.964933 allure-robotframework-2.9.45/examples/description/
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/description/testcase_description.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.964933 allure-robotframework-2.9.45/examples/fixture/
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/fixture/testcase_fixture.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.964933 allure-robotframework-2.9.45/examples/label/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/label/__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/label/labels_library.py
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/label/testcase_bdd_label.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/label/testcase_custom_labels.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.964933 allure-robotframework-2.9.45/examples/link/
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/link/dynamic_link.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/link/link.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/examples/status/
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/status/status.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/status/status_library.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/examples/step/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/step/builtin_step.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/step/outside_step.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/step/outside_step_library.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/examples/tag/
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/tag/tag.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/examples/testplan/
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/examples/testplan/testplan.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.960933 allure-robotframework-2.9.45/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/src/library/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/library/allure_library.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/src/listener/
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/listener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10936 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/listener/allure_listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/listener/allure_testplan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/listener/robot_listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/listener/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/src/listener/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/test/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/test/attach/
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/attach/data_attach.robot
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/attach/file_attach.robot
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/attach/foreign_library_attach.robot
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.968933 allure-robotframework-2.9.45/test/description/
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/description/testcase_description.robot
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/fixture/suite_fixture.robot
+-rw-r--r--   0 runner    (1001) docker     (121)     2675 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/fixture/testcase_fixture.robot
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/test/label/
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/label/testcase_bdd_label.robot
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/label/testcase_custom_labels.robot
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/test/link/
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/link/dynamic_link.robot
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/link/link.robot
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/link/suite_link.robot
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/run_robot_library.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/test/status/
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/status/status.robot
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/test/step/
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/step/builtin_step.robot
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/step/outside_step.robot
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/test/tag/
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/tag/tag.robot
+-rw-r--r--   0 runner    (1001) docker     (121)     4966 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/test_allure_library.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:36.972933 allure-robotframework-2.9.45/test/testplan/
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/test/testplan/testplan.robot
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2021-10-15 08:21:54.000000 allure-robotframework-2.9.45/tox.ini
```

### Comparing `allure-robotframework-2.9.44/PKG-INFO` & `allure-robotframework-2.9.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-robotframework
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure Robot Framework integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: Sergey Khomutinin
 Author-email: skhomuti@gmail.com
 License: Apache-2.0
 Keywords: allure reporting robotframework
 Platform: UNKNOWN
```

### Comparing `allure-robotframework-2.9.44/README.rst` & `allure-robotframework-2.9.45/README.rst`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/allure_robotframework.egg-info/PKG-INFO` & `allure-robotframework-2.9.45/allure_robotframework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-robotframework
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure Robot Framework integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: Sergey Khomutinin
 Author-email: skhomuti@gmail.com
 License: Apache-2.0
 Keywords: allure reporting robotframework
 Platform: UNKNOWN
```

### Comparing `allure-robotframework-2.9.44/allure_robotframework.egg-info/SOURCES.txt` & `allure-robotframework-2.9.45/allure_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/examples/attach/foreign_library_attach.rst` & `allure-robotframework-2.9.45/examples/attach/foreign_library_attach.rst`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/examples/attach/foreign_library_helper.py` & `allure-robotframework-2.9.45/examples/attach/foreign_library_helper.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/examples/description/testcase_description.rst` & `allure-robotframework-2.9.45/examples/description/testcase_description.rst`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/examples/fixture/testcase_fixture.rst` & `allure-robotframework-2.9.45/examples/fixture/testcase_fixture.rst`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/examples/link/link.rst` & `allure-robotframework-2.9.45/examples/link/link.rst`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/examples/tag/tag.rst` & `allure-robotframework-2.9.45/examples/tag/tag.rst`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/setup.py` & `allure-robotframework-2.9.45/setup.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/src/library/allure_library.py` & `allure-robotframework-2.9.45/src/library/allure_library.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/src/listener/allure_listener.py` & `allure-robotframework-2.9.45/src/listener/allure_listener.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/src/listener/allure_testplan.py` & `allure-robotframework-2.9.45/src/listener/allure_testplan.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/src/listener/robot_listener.py` & `allure-robotframework-2.9.45/src/listener/robot_listener.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/src/listener/utils.py` & `allure-robotframework-2.9.45/src/listener/utils.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/attach/data_attach.robot` & `allure-robotframework-2.9.45/test/attach/data_attach.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/attach/foreign_library_attach.robot` & `allure-robotframework-2.9.45/test/attach/foreign_library_attach.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/description/testcase_description.robot` & `allure-robotframework-2.9.45/test/description/testcase_description.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/fixture/testcase_fixture.robot` & `allure-robotframework-2.9.45/test/fixture/testcase_fixture.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/link/dynamic_link.robot` & `allure-robotframework-2.9.45/test/link/dynamic_link.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/link/link.robot` & `allure-robotframework-2.9.45/test/link/link.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/link/suite_link.robot` & `allure-robotframework-2.9.45/test/link/suite_link.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/run_robot_library.py` & `allure-robotframework-2.9.45/test/run_robot_library.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/status/status.robot` & `allure-robotframework-2.9.45/test/status/status.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/step/builtin_step.robot` & `allure-robotframework-2.9.45/test/step/builtin_step.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/tag/tag.robot` & `allure-robotframework-2.9.45/test/tag/tag.robot`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/test/test_allure_library.py` & `allure-robotframework-2.9.45/test/test_allure_library.py`

 * *Files identical despite different names*

### Comparing `allure-robotframework-2.9.44/tox.ini` & `allure-robotframework-2.9.45/tox.ini`

 * *Files identical despite different names*

