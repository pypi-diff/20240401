# Comparing `tmp/allure-pytest-2.9.44.tar.gz` & `tmp/allure-pytest-2.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allure-pytest-2.9.44.tar", last modified: Wed Sep 29 20:24:32 2021, max compression
+gzip compressed data, was "allure-pytest-2.9.45.tar", last modified: Fri Oct 15 08:22:27 2021, max compression
```

## Comparing `allure-pytest-2.9.44.tar` & `allure-pytest-2.9.45.tar`

### file list

```diff
@@ -1,170 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.713684 allure-pytest-2.9.44/
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-09-29 20:24:32.713684 allure-pytest-2.9.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/allure_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-09-29 20:24:32.000000 allure-pytest-2.9.44/allure_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5253 2021-09-29 20:24:32.000000 allure-pytest-2.9.44/allure_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 20:24:32.000000 allure-pytest-2.9.44/allure_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-09-29 20:24:32.000000 allure-pytest-2.9.44/allure_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-09-29 20:24:32.000000 allure-pytest-2.9.44/allure_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-29 20:24:32.000000 allure-pytest-2.9.44/allure_pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.697684 allure-pytest-2.9.44/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/attachment/
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/attachment/attachment.rst
--rw-r--r--   0 runner    (1001) docker     (121)      762 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/attachment/attachment_fixture.rst
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/attachment/attachment_step.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/description/
--rw-r--r--   0 runner    (1001) docker     (121)      889 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/description/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      513 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/description/dynamic_description.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/display_name/
--rw-r--r--   0 runner    (1001) docker     (121)      469 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/display_name/display_name.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/display_name/dynamic_display_name.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.697684 allure-pytest-2.9.44/examples/label/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/label/bdd/
--rw-r--r--   0 runner    (1001) docker     (121)      585 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/bdd/bdd_label.rst
--rw-r--r--   0 runner    (1001) docker     (121)      396 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/bdd/dynamic_bdd_label.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/bdd/select_tests_by_bdd.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/label/custom/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/custom/custom_label.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/label/severity/
--rw-r--r--   0 runner    (1001) docker     (121)      832 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/severity/class_severity.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/severity/module_severity.rst
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/severity/select_tests_by_severity.rst
--rw-r--r--   0 runner    (1001) docker     (121)      372 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/severity/severity.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/label/suite/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/suite/custom_suite.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/label/suite/module_level_custom_suite.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/link/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/link/dynamic_link.rst
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/link/link.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.701685 allure-pytest-2.9.44/examples/step/
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/step/step.rst
--rw-r--r--   0 runner    (1001) docker     (121)      936 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/examples/step/step_placeholder.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 20:24:32.713684 allure-pytest-2.9.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/src/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    12831 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/src/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     9011 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/src/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     6082 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/attachment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/attachment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/attachment/attachment_class_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/attachment/attachment_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/attachment/attachment_hook_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/attachment/attachment_parametrized_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/attachment/attachment_step_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/attachment/attachment_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/capture/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4061 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/capture/capture_attach_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/description/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/description/description_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      871 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/description/dynamic_description_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/display_name/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/display_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/display_name/display_name_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/display_name/dynamic_display_name_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/duration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/duration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/duration/duration_time_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/fixture/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/fixture/fixture_finalized_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9731 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/fixture/fixture_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/fixture/function_scope/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/fixture/function_scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/fixture/parametrized_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/fixture/yield_fixture_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/history_id/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/history_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/history_id/history_id_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/label/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/label/bdd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/bdd/bdd_label_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/bdd/dynamic_bdd_label_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/bdd/select_bdd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/label/custom/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/custom/custom_label_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.705685 allure-pytest-2.9.44/test/acceptance/label/package/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/package/regression_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/label/severity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/severity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/severity/class_severity_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/severity/module_severity_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/severity/select_severity_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/severity/severity_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/label/suite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/suite/custom_suite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/suite/default_suite_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/suite/module_level_custom_suite_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/label/tag/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/label/tag/tag_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/link/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/link/dynamic_link_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/link/link_pattern_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/link/link_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/parametrization/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/parametrization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/parametrization/metafunc_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/parametrization/parametrization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/status/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/base_call_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7298 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/base_setup_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/base_step_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/base_teardown_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/skip_call_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/skip_setup_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/skip_step_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/skip_teardown_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/xfail_call_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/xfail_setup_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/xfail_step_status_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/status/xfail_teardown_status_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/step/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/step/outside_step_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/step/step_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/step/step_placeholder_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/step/step_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/acceptance/unicode_identifier/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/unicode_identifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/acceptance/unicode_identifier/unicode_identifier_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3025 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/integration/allure_ee/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/allure_ee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/allure_ee/select_test_from_testplan_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/allure_ee/set_testcase_id_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/integration/pytest_doctest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_doctest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_doctest/pytest_doctest_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/integration/pytest_flakes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_flakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_flakes/pytest_flakes_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/integration/pytest_lazy_fixture/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_lazy_fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_lazy_fixture/pytest_lazy_fixture_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.709684 allure-pytest-2.9.44/test/integration/pytest_rerunfailures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_rerunfailures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_rerunfailures/pytest_rerunfailures_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:32.713684 allure-pytest-2.9.44/test/integration/pytest_xdist/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_xdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/test/integration/pytest_xdist/pytest_xdist_select_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2021-09-29 20:24:05.000000 allure-pytest-2.9.44/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.860883 allure-pytest-2.9.45/
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-10-15 08:22:27.860883 allure-pytest-2.9.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/allure_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-10-15 08:22:27.000000 allure-pytest-2.9.45/allure_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5346 2021-10-15 08:22:27.000000 allure-pytest-2.9.45/allure_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 08:22:27.000000 allure-pytest-2.9.45/allure_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-15 08:22:27.000000 allure-pytest-2.9.45/allure_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-15 08:22:27.000000 allure-pytest-2.9.45/allure_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-15 08:22:27.000000 allure-pytest-2.9.45/allure_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.836883 allure-pytest-2.9.45/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/attachment/
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/attachment/attachment.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/attachment/attachment_fixture.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/attachment/attachment_step.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/description/
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/description/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/description/dynamic_description.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/display_name/
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/display_name/display_name.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/display_name/dynamic_display_name.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.836883 allure-pytest-2.9.45/examples/label/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/label/bdd/
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/bdd/bdd_label.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/bdd/dynamic_bdd_label.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/bdd/select_tests_by_bdd.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/label/custom/
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/custom/custom_label.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/label/severity/
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/severity/class_severity.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/severity/module_severity.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/severity/select_tests_by_severity.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/severity/severity.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/label/suite/
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/suite/custom_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/label/suite/module_level_custom_suite.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/link/
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/link/dynamic_link.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/link/link.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.840883 allure-pytest-2.9.45/examples/step/
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/step/step.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/examples/step/step_placeholder.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 08:22:27.860883 allure-pytest-2.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2089 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.844883 allure-pytest-2.9.45/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/src/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12831 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/src/listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9955 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/src/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6082 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.844883 allure-pytest-2.9.45/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.844883 allure-pytest-2.9.45/test/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.844883 allure-pytest-2.9.45/test/acceptance/attachment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/attachment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/attachment/attachment_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/attachment/attachment_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/attachment/attachment_hook_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/attachment/attachment_parametrized_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/attachment/attachment_step_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/attachment/attachment_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.844883 allure-pytest-2.9.45/test/acceptance/capture/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4061 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/capture/capture_attach_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.844883 allure-pytest-2.9.45/test/acceptance/description/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/description/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/description/dynamic_description_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.844883 allure-pytest-2.9.45/test/acceptance/display_name/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/display_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/display_name/display_name_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/display_name/dynamic_display_name_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/duration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/duration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2708 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/duration/duration_time_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/fixture/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3070 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/fixture/fixture_finalized_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9731 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/fixture/fixture_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/fixture/function_scope/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/fixture/function_scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/fixture/parametrized_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/fixture/yield_fixture_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/history_id/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/history_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/history_id/history_id_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/label/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/label/bdd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/bdd/bdd_label_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/bdd/dynamic_bdd_label_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/bdd/select_bdd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/label/custom/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/custom/custom_label_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.848883 allure-pytest-2.9.45/test/acceptance/label/package/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/package/regression_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.852883 allure-pytest-2.9.45/test/acceptance/label/severity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/severity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/severity/class_severity_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/severity/module_severity_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/severity/select_severity_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/severity/severity_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.852883 allure-pytest-2.9.45/test/acceptance/label/suite/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/suite/custom_suite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/suite/default_suite_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/suite/module_level_custom_suite_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.852883 allure-pytest-2.9.45/test/acceptance/label/tag/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4121 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/label/tag/tag_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.852883 allure-pytest-2.9.45/test/acceptance/link/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1780 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/link/dynamic_link_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/link/link_pattern_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/link/link_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.852883 allure-pytest-2.9.45/test/acceptance/parametrization/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/parametrization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/parametrization/metafunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3344 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/parametrization/parametrization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.856883 allure-pytest-2.9.45/test/acceptance/status/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/base_call_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7298 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/base_setup_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3804 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/base_step_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3745 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/base_teardown_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2691 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/skip_call_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1699 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/skip_setup_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1292 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/skip_step_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/skip_teardown_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4151 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/xfail_call_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/xfail_setup_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/xfail_step_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/status/xfail_teardown_status_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.856883 allure-pytest-2.9.45/test/acceptance/step/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/step/outside_step_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1777 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/step/step_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/step/step_placeholder_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/step/step_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.856883 allure-pytest-2.9.45/test/acceptance/unicode_identifier/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/unicode_identifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/acceptance/unicode_identifier/unicode_identifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3025 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.856883 allure-pytest-2.9.45/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.856883 allure-pytest-2.9.45/test/integration/allure_ee/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/allure_ee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2785 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/allure_ee/select_test_from_testplan_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/allure_ee/set_testcase_id_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.856883 allure-pytest-2.9.45/test/integration/pytest_check/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_check/pytest_check_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.856883 allure-pytest-2.9.45/test/integration/pytest_doctest/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_doctest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_doctest/pytest_doctest_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.860883 allure-pytest-2.9.45/test/integration/pytest_flakes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_flakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_flakes/pytest_flakes_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.860883 allure-pytest-2.9.45/test/integration/pytest_lazy_fixture/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_lazy_fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_lazy_fixture/pytest_lazy_fixture_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.860883 allure-pytest-2.9.45/test/integration/pytest_rerunfailures/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_rerunfailures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_rerunfailures/pytest_rerunfailures_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:27.860883 allure-pytest-2.9.45/test/integration/pytest_xdist/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_xdist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/test/integration/pytest_xdist/pytest_xdist_select_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2345 2021-10-15 08:21:54.000000 allure-pytest-2.9.45/tox.ini
```

### Comparing `allure-pytest-2.9.44/PKG-INFO` & `allure-pytest-2.9.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-pytest
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure pytest integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting pytest
 Platform: UNKNOWN
```

### Comparing `allure-pytest-2.9.44/README.rst` & `allure-pytest-2.9.45/README.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/allure_pytest.egg-info/PKG-INFO` & `allure-pytest-2.9.45/allure_pytest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-pytest
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure pytest integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting pytest
 Platform: UNKNOWN
```

### Comparing `allure-pytest-2.9.44/allure_pytest.egg-info/SOURCES.txt` & `allure-pytest-2.9.45/allure_pytest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,16 @@
 test/acceptance/step/step_test.py
 test/acceptance/unicode_identifier/__init__.py
 test/acceptance/unicode_identifier/unicode_identifier_test.py
 test/integration/__init__.py
 test/integration/allure_ee/__init__.py
 test/integration/allure_ee/select_test_from_testplan_test.py
 test/integration/allure_ee/set_testcase_id_test.py
+test/integration/pytest_check/__init__.py
+test/integration/pytest_check/pytest_check_test.py
 test/integration/pytest_doctest/__init__.py
 test/integration/pytest_doctest/pytest_doctest_test.py
 test/integration/pytest_flakes/__init__.py
 test/integration/pytest_flakes/pytest_flakes_test.py
 test/integration/pytest_lazy_fixture/__init__.py
 test/integration/pytest_lazy_fixture/pytest_lazy_fixture_test.py
 test/integration/pytest_rerunfailures/__init__.py
```

### Comparing `allure-pytest-2.9.44/examples/attachment/attachment.rst` & `allure-pytest-2.9.45/examples/attachment/attachment.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/attachment/attachment_fixture.rst` & `allure-pytest-2.9.45/examples/attachment/attachment_fixture.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/description/description.rst` & `allure-pytest-2.9.45/examples/description/description.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/description/dynamic_description.rst` & `allure-pytest-2.9.45/examples/description/dynamic_description.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/label/bdd/bdd_label.rst` & `allure-pytest-2.9.45/examples/label/bdd/bdd_label.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/label/bdd/select_tests_by_bdd.rst` & `allure-pytest-2.9.45/examples/label/bdd/select_tests_by_bdd.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/label/severity/class_severity.rst` & `allure-pytest-2.9.45/examples/label/severity/class_severity.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/label/severity/module_severity.rst` & `allure-pytest-2.9.45/examples/label/severity/module_severity.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/label/severity/select_tests_by_severity.rst` & `allure-pytest-2.9.45/examples/label/severity/select_tests_by_severity.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/step/step.rst` & `allure-pytest-2.9.45/examples/step/step.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/examples/step/step_placeholder.rst` & `allure-pytest-2.9.45/examples/step/step_placeholder.rst`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/setup.py` & `allure-pytest-2.9.45/setup.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/src/helper.py` & `allure-pytest-2.9.45/src/helper.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/src/listener.py` & `allure-pytest-2.9.45/src/listener.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/src/plugin.py` & `allure-pytest-2.9.45/src/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,20 @@
                                            help="Clean alluredir folder if it exists")
 
     parser.getgroup("reporting").addoption('--allure-no-capture',
                                            action="store_false",
                                            dest="attach_capture",
                                            help="Do not attach pytest captured logging/stdout/stderr to report")
 
+    parser.getgroup("reporting").addoption('--inversion',
+                                           action="store",
+                                           dest="inversion",
+                                           default=False,
+                                           help="Run tests not in testplan")
+
     def label_type(type_name, legal_values=set()):
         def a_label_type(string):
             atoms = set(string.split(','))
             if type_name is LabelType.SEVERITY:
                 if not atoms < legal_values:
                     raise argparse.ArgumentTypeError('Illegal {} values: {}, only [{}] are allowed'.format(
                         type_name, ', '.join(atoms - legal_values), ', '.join(legal_values)))
@@ -152,36 +158,51 @@
 
 def select_by_labels(items, config):
     arg_labels = set().union(config.option.allure_epics,
                              config.option.allure_features,
                              config.option.allure_stories,
                              config.option.allure_ids,
                              config.option.allure_severities)
-    return filter(lambda item: arg_labels & set(allure_labels(item)) if arg_labels else True, items)
+    if arg_labels:
+        selected, deselected = [], []
+        for item in items:
+            selected.append(item) if arg_labels & set(allure_labels(item)) else deselected.append(item)
+        return selected, deselected
+    else:
+        return items, []
 
 
-def select_by_testcase(items):
+def select_by_testcase(items, config):
     planned_tests = get_testplan()
+    is_inversion = config.option.inversion
 
     if planned_tests:
 
         def is_planed(item):
             allure_ids = allure_label(item, LabelType.ID)
             allure_string_ids = list(map(str, allure_ids))
             for planed_item in planned_tests:
                 planed_item_string_id = str(planed_item.get("id"))
                 planed_item_selector = planed_item.get("selector")
                 if (
                     planed_item_string_id in allure_string_ids
                     or planed_item_selector == allure_full_name(item)
                 ):
-                    return True
-            return False
+                    return True if not is_inversion else False
+            return False if not is_inversion else True
 
-        return [item for item in items if is_planed(item)]
+        selected, deselected = [], []
+        for item in items:
+            selected.append(item) if is_planed(item) else deselected.append(item)
+        return selected, deselected
     else:
-        return items
+        return items, []
 
 
 def pytest_collection_modifyitems(items, config):
-    items[:] = select_by_testcase(items)
-    items[:] = select_by_labels(items, config)
+    selected, deselected_by_testcase = select_by_testcase(items, config)
+    selected, deselected_by_labels = select_by_labels(selected, config)
+
+    items[:] = selected
+
+    if deselected_by_testcase or deselected_by_labels:
+        config.hook.pytest_deselected(items=[*deselected_by_testcase, *deselected_by_labels])
```

### Comparing `allure-pytest-2.9.44/src/utils.py` & `allure-pytest-2.9.45/src/utils.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/attachment/attachment_class_test.py` & `allure-pytest-2.9.45/test/acceptance/attachment/attachment_class_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/attachment/attachment_fixture_test.py` & `allure-pytest-2.9.45/test/acceptance/attachment/attachment_fixture_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/attachment/attachment_hook_test.py` & `allure-pytest-2.9.45/test/acceptance/attachment/attachment_hook_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/attachment/attachment_parametrized_test.py` & `allure-pytest-2.9.45/test/acceptance/attachment/attachment_parametrized_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/attachment/attachment_step_test.py` & `allure-pytest-2.9.45/test/acceptance/attachment/attachment_step_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/attachment/attachment_test.py` & `allure-pytest-2.9.45/test/acceptance/attachment/attachment_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/capture/capture_attach_test.py` & `allure-pytest-2.9.45/test/acceptance/capture/capture_attach_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/description/description_test.py` & `allure-pytest-2.9.45/test/acceptance/description/description_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/description/dynamic_description_test.py` & `allure-pytest-2.9.45/test/acceptance/description/dynamic_description_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/display_name/display_name_test.py` & `allure-pytest-2.9.45/test/acceptance/display_name/display_name_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/duration/duration_time_test.py` & `allure-pytest-2.9.45/test/acceptance/duration/duration_time_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/fixture/fixture_finalized_test.py` & `allure-pytest-2.9.45/test/acceptance/fixture/fixture_finalized_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/fixture/fixture_test.py` & `allure-pytest-2.9.45/test/acceptance/fixture/fixture_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/fixture/parametrized_fixture_test.py` & `allure-pytest-2.9.45/test/acceptance/fixture/parametrized_fixture_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/fixture/yield_fixture_test.py` & `allure-pytest-2.9.45/test/acceptance/fixture/yield_fixture_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/history_id/history_id_test.py` & `allure-pytest-2.9.45/test/acceptance/history_id/history_id_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/bdd/bdd_label_test.py` & `allure-pytest-2.9.45/test/acceptance/label/bdd/bdd_label_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/bdd/dynamic_bdd_label_test.py` & `allure-pytest-2.9.45/test/acceptance/label/bdd/dynamic_bdd_label_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/bdd/select_bdd_test.py` & `allure-pytest-2.9.45/test/acceptance/label/bdd/select_bdd_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/custom/custom_label_test.py` & `allure-pytest-2.9.45/test/acceptance/label/custom/custom_label_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/package/regression_test.py` & `allure-pytest-2.9.45/test/acceptance/label/package/regression_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/severity/class_severity_test.py` & `allure-pytest-2.9.45/test/acceptance/label/severity/class_severity_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/severity/module_severity_test.py` & `allure-pytest-2.9.45/test/acceptance/label/severity/module_severity_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/severity/select_severity_test.py` & `allure-pytest-2.9.45/test/acceptance/label/severity/select_severity_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/suite/custom_suite.py` & `allure-pytest-2.9.45/test/acceptance/label/suite/custom_suite.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/suite/default_suite_test.py` & `allure-pytest-2.9.45/test/acceptance/label/suite/default_suite_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/label/tag/tag_test.py` & `allure-pytest-2.9.45/test/acceptance/label/tag/tag_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/link/dynamic_link_test.py` & `allure-pytest-2.9.45/test/acceptance/link/dynamic_link_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/link/link_pattern_test.py` & `allure-pytest-2.9.45/test/acceptance/link/link_pattern_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/link/link_test.py` & `allure-pytest-2.9.45/test/acceptance/link/link_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/parametrization/metafunc_test.py` & `allure-pytest-2.9.45/test/acceptance/parametrization/metafunc_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/parametrization/parametrization_test.py` & `allure-pytest-2.9.45/test/acceptance/parametrization/parametrization_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/base_call_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/base_call_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/base_setup_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/base_setup_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/base_step_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/base_step_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/base_teardown_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/base_teardown_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/skip_call_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/skip_call_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/skip_setup_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/skip_setup_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/skip_step_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/skip_step_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/skip_teardown_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/skip_teardown_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/xfail_call_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/xfail_call_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/xfail_setup_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/xfail_setup_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/xfail_step_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/xfail_step_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/status/xfail_teardown_status_test.py` & `allure-pytest-2.9.45/test/acceptance/status/xfail_teardown_status_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/step/outside_step_test.py` & `allure-pytest-2.9.45/test/acceptance/step/outside_step_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/step/step_parameters.py` & `allure-pytest-2.9.45/test/acceptance/step/step_parameters.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/step/step_placeholder_test.py` & `allure-pytest-2.9.45/test/acceptance/step/step_placeholder_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/step/step_test.py` & `allure-pytest-2.9.45/test/acceptance/step/step_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/acceptance/unicode_identifier/unicode_identifier_test.py` & `allure-pytest-2.9.45/test/acceptance/unicode_identifier/unicode_identifier_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/conftest.py` & `allure-pytest-2.9.45/test/conftest.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/integration/allure_ee/select_test_from_testplan_test.py` & `allure-pytest-2.9.45/test/integration/allure_ee/select_test_from_testplan_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/integration/allure_ee/set_testcase_id_test.py` & `allure-pytest-2.9.45/test/integration/allure_ee/set_testcase_id_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/integration/pytest_doctest/pytest_doctest_test.py` & `allure-pytest-2.9.45/test/integration/pytest_doctest/pytest_doctest_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/integration/pytest_flakes/pytest_flakes_test.py` & `allure-pytest-2.9.45/test/integration/pytest_flakes/pytest_flakes_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/integration/pytest_lazy_fixture/pytest_lazy_fixture_test.py` & `allure-pytest-2.9.45/test/integration/pytest_lazy_fixture/pytest_lazy_fixture_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/integration/pytest_rerunfailures/pytest_rerunfailures_test.py` & `allure-pytest-2.9.45/test/integration/pytest_rerunfailures/pytest_rerunfailures_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/test/integration/pytest_xdist/pytest_xdist_select_test.py` & `allure-pytest-2.9.45/test/integration/pytest_xdist/pytest_xdist_select_test.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-2.9.44/tox.ini` & `allure-pytest-2.9.45/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 setenv = ALLURE_INDENT_OUTPUT=yep
 
 deps =
     {distshare}/allure-python-commons-test-?.*.zip
     {distshare}/allure-python-commons-?.*.zip
     pyhamcrest
     mock
+    pytest-check
     pytest-flakes
     pytest-rerunfailures
     pytest-xdist
     pytest-lazy-fixture
 
 commands =
     py.test --basetemp={envtmpdir}/tmp \
@@ -34,14 +35,15 @@
 
 basepython = python3.6
 
 setenv = ALLURE_INDENT_OUTPUT=yep
 
 deps =
     pyhamcrest
+    pytest-check
     pytest-flakes
     pytest-rerunfailures
     pytest-xdist
     pytest-lazy-fixture
     mock
     {distshare}/allure-python-commons-2*.zip
     {distshare}/allure-python-commons-test-2*.zip
```

