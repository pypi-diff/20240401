# Comparing `tmp/nrobo-2024.37.0.tar.gz` & `tmp/nrobo-2024.38.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrobo-2024.37.0.tar", last modified: Sun Mar 31 13:45:03 2024, max compression
+gzip compressed data, was "nrobo-2024.38.0.tar", last modified: Mon Apr  1 11:58:58 2024, max compression
```

## Comparing `nrobo-2024.37.0.tar` & `nrobo-2024.38.0.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.669975 nrobo-2024.37.0/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.37.0/LICENSE
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18166 2024-03-31 13:45:03.669448 nrobo-2024.37.0/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16528 2024-03-31 13:37:53.000000 nrobo-2024.37.0/README.rst
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.643683 nrobo-2024.37.0/nrobo/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8668 2024-03-31 13:44:50.000000 nrobo-2024.37.0/nrobo/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.647762 nrobo-2024.37.0/nrobo/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.37.0/nrobo/appium/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.37.0/nrobo/appium/android_capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.37.0/nrobo/appium/ios_capability.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.649463 nrobo-2024.37.0/nrobo/browserConfigs/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/browserConfigs/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/browserConfigs/capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.37.0/nrobo/browserConfigs/chrome_config.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/browserConfigs/chrome_prefs.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/browserConfigs/markers.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.649783 nrobo-2024.37.0/nrobo/browsers/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.37.0/nrobo/browsers/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.650102 nrobo-2024.37.0/nrobo/browsers/chrome/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.37.0/nrobo/browsers/chrome/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.650433 nrobo-2024.37.0/nrobo/browsers/edge/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.37.0/nrobo/browsers/edge/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.650748 nrobo-2024.37.0/nrobo/browsers/firefox/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/browsers/firefox/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.651058 nrobo-2024.37.0/nrobo/browsers/safari/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/browsers/safari/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.652811 nrobo-2024.37.0/nrobo/cli/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.37.0/nrobo/cli/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.37.0/nrobo/cli/cli_constants.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.37.0/nrobo/cli/cli_version.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.653131 nrobo-2024.37.0/nrobo/cli/detection/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/cli/detection/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.653449 nrobo-2024.37.0/nrobo/cli/formatting/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/cli/formatting/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.654159 nrobo-2024.37.0/nrobo/cli/install/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.37.0/nrobo/cli/install/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      945 2024-03-30 00:44:07.000000 nrobo-2024.37.0/nrobo/cli/install/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.37.0/nrobo/cli/launcher.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.654474 nrobo-2024.37.0/nrobo/cli/ncodes/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/cli/ncodes/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.37.0/nrobo/cli/nglobals.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.654798 nrobo-2024.37.0/nrobo/cli/nrobo_args/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.37.0/nrobo/cli/nrobo_args/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.655176 nrobo-2024.37.0/nrobo/cli/tools/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/cli/tools/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.655488 nrobo-2024.37.0/nrobo/cli/upgrade/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.37.0/nrobo/cli/upgrade/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32167 2024-03-31 13:44:50.000000 nrobo-2024.37.0/nrobo/conftest.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.655817 nrobo-2024.37.0/nrobo/exceptions/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/exceptions/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.657337 nrobo-2024.37.0/nrobo/framework/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.37.0/nrobo/framework/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.37.0/nrobo/framework/conftest-host.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.37.0/nrobo/framework/nrobo-config.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.658226 nrobo-2024.37.0/nrobo/framework/pages/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/pages/PagePyPiHome.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/pages/PageSearch.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/pages/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.37.0/nrobo/framework/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.37.0/nrobo/framework/secrets.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.658542 nrobo-2024.37.0/nrobo/framework/tests/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.37.0/nrobo/framework/tests/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.638663 nrobo-2024.37.0/nrobo/framework/tests/mobile/
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.658861 nrobo-2024.37.0/nrobo/framework/tests/mobile/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.37.0/nrobo/framework/tests/mobile/appium/test_appium.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.659188 nrobo-2024.37.0/nrobo/framework/tests/web/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/PyPi_home_page_test.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.659513 nrobo-2024.37.0/nrobo/framework/tests/web/examples/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/examples/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.660168 nrobo-2024.37.0/nrobo/framework/tests/web/gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.37.0/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.37.0/nrobo/framework/tests/web/gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.660423 nrobo-2024.37.0/nrobo/framework/tests/web/no_gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.37.0/nrobo/framework/tests/web/no_gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.662746 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7583 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.663092 nrobo-2024.37.0/nrobo/selenese/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    46353 2024-03-20 04:44:36.000000 nrobo-2024.37.0/nrobo/selenese/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.663533 nrobo-2024.37.0/nrobo/util/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.37.0/nrobo/util/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.663886 nrobo-2024.37.0/nrobo/util/commands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.37.0/nrobo/util/commands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.664227 nrobo-2024.37.0/nrobo/util/commands/ncommands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.37.0/nrobo/util/commands/ncommands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.664564 nrobo-2024.37.0/nrobo/util/commands/posix/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/util/commands/posix/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.664882 nrobo-2024.37.0/nrobo/util/commands/windows/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/util/commands/windows/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.665192 nrobo-2024.37.0/nrobo/util/common/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.37.0/nrobo/util/common/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.665507 nrobo-2024.37.0/nrobo/util/constants/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/util/constants/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.666080 nrobo-2024.37.0/nrobo/util/database/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.37.0/nrobo/util/database/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.37.0/nrobo/util/database/connectors.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.666393 nrobo-2024.37.0/nrobo/util/filesystem/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/util/filesystem/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.666704 nrobo-2024.37.0/nrobo/util/network/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/util/network/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.667010 nrobo-2024.37.0/nrobo/util/platform/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/util/platform/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.667313 nrobo-2024.37.0/nrobo/util/process/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/util/process/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.667623 nrobo-2024.37.0/nrobo/util/python/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/util/python/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.667932 nrobo-2024.37.0/nrobo/util/regex/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.37.0/nrobo/util/regex/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.668236 nrobo-2024.37.0/nrobo/util/version/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.37.0/nrobo/util/version/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-31 13:45:03.668712 nrobo-2024.37.0/nrobo.egg-info/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18166 2024-03-31 13:45:03.000000 nrobo-2024.37.0/nrobo.egg-info/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2776 2024-03-31 13:45:03.000000 nrobo-2024.37.0/nrobo.egg-info/SOURCES.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-03-31 13:45:03.000000 nrobo-2024.37.0/nrobo.egg-info/dependency_links.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-03-31 13:45:03.000000 nrobo-2024.37.0/nrobo.egg-info/entry_points.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-03-31 13:45:03.000000 nrobo-2024.37.0/nrobo.egg-info/requires.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-03-31 13:45:03.000000 nrobo-2024.37.0/nrobo.egg-info/top_level.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-03-31 13:44:50.000000 nrobo-2024.37.0/pyproject.toml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-03-31 13:45:03.670062 nrobo-2024.37.0/setup.cfg
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.183879 nrobo-2024.38.0/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.38.0/LICENSE
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18166 2024-04-01 11:58:58.183298 nrobo-2024.38.0/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16528 2024-04-01 11:54:19.000000 nrobo-2024.38.0/README.rst
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.145610 nrobo-2024.38.0/nrobo/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8668 2024-04-01 11:58:44.000000 nrobo-2024.38.0/nrobo/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.148500 nrobo-2024.38.0/nrobo/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.38.0/nrobo/appium/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.38.0/nrobo/appium/android_capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.38.0/nrobo/appium/ios_capability.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.150451 nrobo-2024.38.0/nrobo/browserConfigs/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/browserConfigs/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/browserConfigs/capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.38.0/nrobo/browserConfigs/chrome_config.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/browserConfigs/chrome_prefs.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/browserConfigs/markers.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.150764 nrobo-2024.38.0/nrobo/browsers/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.38.0/nrobo/browsers/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.151068 nrobo-2024.38.0/nrobo/browsers/chrome/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.38.0/nrobo/browsers/chrome/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.151374 nrobo-2024.38.0/nrobo/browsers/edge/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.38.0/nrobo/browsers/edge/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.151872 nrobo-2024.38.0/nrobo/browsers/firefox/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/browsers/firefox/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.152387 nrobo-2024.38.0/nrobo/browsers/safari/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/browsers/safari/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.155179 nrobo-2024.38.0/nrobo/cli/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.38.0/nrobo/cli/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.38.0/nrobo/cli/cli_constants.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.38.0/nrobo/cli/cli_version.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.155670 nrobo-2024.38.0/nrobo/cli/detection/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/cli/detection/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.156140 nrobo-2024.38.0/nrobo/cli/formatting/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/cli/formatting/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.157555 nrobo-2024.38.0/nrobo/cli/install/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.38.0/nrobo/cli/install/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      945 2024-03-30 00:44:07.000000 nrobo-2024.38.0/nrobo/cli/install/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.38.0/nrobo/cli/launcher.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.158224 nrobo-2024.38.0/nrobo/cli/ncodes/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/cli/ncodes/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.38.0/nrobo/cli/nglobals.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.158905 nrobo-2024.38.0/nrobo/cli/nrobo_args/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.38.0/nrobo/cli/nrobo_args/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.168815 nrobo-2024.38.0/nrobo/cli/tools/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/cli/tools/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.169300 nrobo-2024.38.0/nrobo/cli/upgrade/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.38.0/nrobo/cli/upgrade/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32167 2024-04-01 11:58:44.000000 nrobo-2024.38.0/nrobo/conftest.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.169677 nrobo-2024.38.0/nrobo/exceptions/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/exceptions/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.171312 nrobo-2024.38.0/nrobo/framework/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.38.0/nrobo/framework/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.38.0/nrobo/framework/conftest-host.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.38.0/nrobo/framework/nrobo-config.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.172384 nrobo-2024.38.0/nrobo/framework/pages/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/pages/PagePyPiHome.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/pages/PageSearch.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/pages/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.38.0/nrobo/framework/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.38.0/nrobo/framework/secrets.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.172738 nrobo-2024.38.0/nrobo/framework/tests/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.38.0/nrobo/framework/tests/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.139910 nrobo-2024.38.0/nrobo/framework/tests/mobile/
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.173059 nrobo-2024.38.0/nrobo/framework/tests/mobile/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.38.0/nrobo/framework/tests/mobile/appium/test_appium.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.173371 nrobo-2024.38.0/nrobo/framework/tests/web/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/PyPi_home_page_test.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.173696 nrobo-2024.38.0/nrobo/framework/tests/web/examples/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/examples/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.174353 nrobo-2024.38.0/nrobo/framework/tests/web/gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.38.0/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.38.0/nrobo/framework/tests/web/gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.174595 nrobo-2024.38.0/nrobo/framework/tests/web/no_gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.38.0/nrobo/framework/tests/web/no_gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.176791 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7583 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.177116 nrobo-2024.38.0/nrobo/selenese/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    46567 2024-04-01 11:49:37.000000 nrobo-2024.38.0/nrobo/selenese/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.177486 nrobo-2024.38.0/nrobo/util/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.38.0/nrobo/util/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.177803 nrobo-2024.38.0/nrobo/util/commands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.38.0/nrobo/util/commands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.178117 nrobo-2024.38.0/nrobo/util/commands/ncommands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.38.0/nrobo/util/commands/ncommands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.178417 nrobo-2024.38.0/nrobo/util/commands/posix/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/util/commands/posix/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.178724 nrobo-2024.38.0/nrobo/util/commands/windows/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/util/commands/windows/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.179028 nrobo-2024.38.0/nrobo/util/common/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.38.0/nrobo/util/common/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.179334 nrobo-2024.38.0/nrobo/util/constants/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/util/constants/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.179884 nrobo-2024.38.0/nrobo/util/database/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.38.0/nrobo/util/database/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.38.0/nrobo/util/database/connectors.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.180192 nrobo-2024.38.0/nrobo/util/filesystem/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/util/filesystem/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.180497 nrobo-2024.38.0/nrobo/util/network/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/util/network/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.180798 nrobo-2024.38.0/nrobo/util/platform/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/util/platform/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.181120 nrobo-2024.38.0/nrobo/util/process/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/util/process/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.181433 nrobo-2024.38.0/nrobo/util/python/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/util/python/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.181742 nrobo-2024.38.0/nrobo/util/regex/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.38.0/nrobo/util/regex/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.182042 nrobo-2024.38.0/nrobo/util/version/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.38.0/nrobo/util/version/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-01 11:58:58.182540 nrobo-2024.38.0/nrobo.egg-info/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18166 2024-04-01 11:58:58.000000 nrobo-2024.38.0/nrobo.egg-info/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2776 2024-04-01 11:58:58.000000 nrobo-2024.38.0/nrobo.egg-info/SOURCES.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-01 11:58:58.000000 nrobo-2024.38.0/nrobo.egg-info/dependency_links.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-01 11:58:58.000000 nrobo-2024.38.0/nrobo.egg-info/entry_points.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-01 11:58:58.000000 nrobo-2024.38.0/nrobo.egg-info/requires.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-01 11:58:58.000000 nrobo-2024.38.0/nrobo.egg-info/top_level.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-01 11:58:44.000000 nrobo-2024.38.0/pyproject.toml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-01 11:58:58.183978 nrobo-2024.38.0/setup.cfg
```

### Comparing `nrobo-2024.37.0/LICENSE` & `nrobo-2024.38.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/PKG-INFO` & `nrobo-2024.38.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.37.0
+Version: 2024.38.0
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,113 +384,113 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.39%
-     - 22,502
+     - 39.34%
+     - 22,712
    * - CN
-     - 13.15%
-     - 7,511
+     - 13.09%
+     - 7,556
    * - DE
-     - 5.83%
-     - 3,330
+     - 6.10%
+     - 3,524
    * - SG
-     - 5.30%
-     - 3,025
+     - 5.28%
+     - 3,047
    * - RU
-     - 5.18%
-     - 2,962
+     - 5.19%
+     - 2,996
    * - HK
-     - 4.24%
-     - 2,420
+     - 4.21%
+     - 2,432
    * - JP
-     - 3.17%
-     - 1,810
+     - 3.15%
+     - 1,818
    * - FR
-     - 2.90%
-     - 1,657
+     - 2.88%
+     - 1,664
    * - KR
-     - 2.78%
+     - 2.75%
      - 1,589
    * - CA
-     - 2.73%
-     - 1,557
+     - 2.72%
+     - 1,569
    * - NO
-     - 1.99%
-     - 1,137
+     - 2.00%
+     - 1,155
    * - GB
      - 1.88%
-     - 1,072
+     - 1,085
    * - AU
-     - 1.79%
-     - 1,023
+     - 1.78%
+     - 1,027
    * - IN
      - 1.52%
-     - 869
+     - 879
    * - SE
      - 1.23%
-     - 702
+     - 708
    * - TH
-     - 0.80%
+     - 0.79%
      - 458
    * - HR
      - 0.79%
-     - 452
+     - 456
    * - DK
-     - 0.69%
+     - 0.68%
      - 395
    * - IE
      - 0.66%
-     - 375
+     - 381
    * - TW
-     - 0.64%
+     - 0.63%
      - 363
    * - IL
      - 0.56%
      - 321
    * - NL
-     - 0.52%
+     - 0.51%
      - 297
    * - ES
-     - 0.46%
+     - 0.45%
      - 262
    * - CH
      - 0.43%
-     - 244
+     - 246
    * - AE
      - 0.35%
-     - 201
+     - 203
    * - FI
      - 0.16%
      - 91
    * - ZA
-     - 0.16%
+     - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.11%
      - 61
-   * - TR
+   * - CW
      - 0.08%
      - 44
-   * - CW
+   * - TR
      - 0.08%
      - 44
-   * - IS
+   * - OM
      - 0.07%
      - 42
-   * - CZ
+   * - IS
      - 0.07%
      - 42
-   * - OM
+   * - CZ
      - 0.07%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
@@ -509,20 +509,20 @@
      - 3
    * - EE
      - 0.01%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
-   * - MX
+   * - RS
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **57,129**
+     - **57,738**
```

### Comparing `nrobo-2024.37.0/README.rst` & `nrobo-2024.38.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -348,113 +348,113 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.39%
-     - 22,502
+     - 39.34%
+     - 22,712
    * - CN
-     - 13.15%
-     - 7,511
+     - 13.09%
+     - 7,556
    * - DE
-     - 5.83%
-     - 3,330
+     - 6.10%
+     - 3,524
    * - SG
-     - 5.30%
-     - 3,025
+     - 5.28%
+     - 3,047
    * - RU
-     - 5.18%
-     - 2,962
+     - 5.19%
+     - 2,996
    * - HK
-     - 4.24%
-     - 2,420
+     - 4.21%
+     - 2,432
    * - JP
-     - 3.17%
-     - 1,810
+     - 3.15%
+     - 1,818
    * - FR
-     - 2.90%
-     - 1,657
+     - 2.88%
+     - 1,664
    * - KR
-     - 2.78%
+     - 2.75%
      - 1,589
    * - CA
-     - 2.73%
-     - 1,557
+     - 2.72%
+     - 1,569
    * - NO
-     - 1.99%
-     - 1,137
+     - 2.00%
+     - 1,155
    * - GB
      - 1.88%
-     - 1,072
+     - 1,085
    * - AU
-     - 1.79%
-     - 1,023
+     - 1.78%
+     - 1,027
    * - IN
      - 1.52%
-     - 869
+     - 879
    * - SE
      - 1.23%
-     - 702
+     - 708
    * - TH
-     - 0.80%
+     - 0.79%
      - 458
    * - HR
      - 0.79%
-     - 452
+     - 456
    * - DK
-     - 0.69%
+     - 0.68%
      - 395
    * - IE
      - 0.66%
-     - 375
+     - 381
    * - TW
-     - 0.64%
+     - 0.63%
      - 363
    * - IL
      - 0.56%
      - 321
    * - NL
-     - 0.52%
+     - 0.51%
      - 297
    * - ES
-     - 0.46%
+     - 0.45%
      - 262
    * - CH
      - 0.43%
-     - 244
+     - 246
    * - AE
      - 0.35%
-     - 201
+     - 203
    * - FI
      - 0.16%
      - 91
    * - ZA
-     - 0.16%
+     - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.11%
      - 61
-   * - TR
+   * - CW
      - 0.08%
      - 44
-   * - CW
+   * - TR
      - 0.08%
      - 44
-   * - IS
+   * - OM
      - 0.07%
      - 42
-   * - CZ
+   * - IS
      - 0.07%
      - 42
-   * - OM
+   * - CZ
      - 0.07%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
@@ -473,20 +473,20 @@
      - 3
    * - EE
      - 0.01%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
-   * - MX
+   * - RS
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **57,129**
+     - **57,738**
```

### Comparing `nrobo-2024.37.0/nrobo/__init__.py` & `nrobo-2024.38.0/nrobo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 nrobo module loads nRoBo globals.
 
 
 @author: Panchdev Singh Chauhan
 @email: erpanchdev@gmail.com
 """
 
-__version__ = '2024.37.0'
+__version__ = '2024.38.0'
 
 # install rich library
 import os
 from pathlib import Path
 
 
 class DB_CONNECTOR_TYPE:
```

### Comparing `nrobo-2024.37.0/nrobo/appium/__init__.py` & `nrobo-2024.38.0/nrobo/appium/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/browsers/chrome/__init__.py` & `nrobo-2024.38.0/nrobo/browsers/chrome/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/__init__.py` & `nrobo-2024.38.0/nrobo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/cli_constants.py` & `nrobo-2024.38.0/nrobo/cli/cli_constants.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/detection/__init__.py` & `nrobo-2024.38.0/nrobo/cli/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/formatting/__init__.py` & `nrobo-2024.38.0/nrobo/cli/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/install/__init__.py` & `nrobo-2024.38.0/nrobo/cli/install/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/install/requirements.txt` & `nrobo-2024.38.0/nrobo/cli/install/requirements.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/launcher.py` & `nrobo-2024.38.0/nrobo/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/ncodes/__init__.py` & `nrobo-2024.38.0/nrobo/cli/ncodes/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/nglobals.py` & `nrobo-2024.38.0/nrobo/cli/nglobals.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/nrobo_args/__init__.py` & `nrobo-2024.38.0/nrobo/cli/nrobo_args/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/tools/__init__.py` & `nrobo-2024.38.0/nrobo/cli/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/cli/upgrade/__init__.py` & `nrobo-2024.38.0/nrobo/cli/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/conftest.py` & `nrobo-2024.38.0/nrobo/conftest.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/exceptions/__init__.py` & `nrobo-2024.38.0/nrobo/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/conftest-host.py` & `nrobo-2024.38.0/nrobo/framework/conftest-host.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/nrobo-config.yaml` & `nrobo-2024.38.0/nrobo/framework/nrobo-config.yaml`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/pages/PagePyPiHome.py` & `nrobo-2024.38.0/nrobo/framework/pages/PagePyPiHome.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/pages/__init__.py` & `nrobo-2024.38.0/nrobo/framework/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/PyPi_home_page_test.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/examples/__init__.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/gui/PyPi_home_page_test.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/gui/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py` & `nrobo-2024.38.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/selenese/__init__.py` & `nrobo-2024.38.0/nrobo/selenese/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -886,16 +886,16 @@
     def submit(self, by: AnyBy, value: Optional[str] = None):
         """Submits a form."""
         self.find_element(by, value).submit()
 
     def clear_spl(self, by: AnyBy, value: Optional[str] = None):
 
         element = self.find_element(by, value)
-        self.action_chain().click(element).send_keys(Keys.ARROW_LEFT)\
-            .double_click(self.find_element(by, value)).send_keys(Keys.DELETE)\
+        self.action_chain().click(element).send_keys(Keys.ARROW_LEFT) \
+            .double_click(self.find_element(by, value)).send_keys(Keys.DELETE) \
             .perform()
         # self.wait_for_a_while(1)
 
     def clear(self, by: AnyBy, value: Optional[str] = None) -> None:
         """Clears the text if it's a text entry element."""
         # self.find_element(by, value).clear()
         self.clear_spl(by, value)
@@ -1135,14 +1135,23 @@
                 lambda driver: driver.execute_script('return document.readyState') == 'complete')
         except TimeoutException as te:
             nprint(f"Exception: {te}", STYLE.HLRed)
         except AttributeError as ae:
             nprint(f"Exception: {ae}", STYLE.HLRed)
         nprint("End of Wait for page load...", style=STYLE.PURPLE4)
 
+    def wait(self, time_in_sec=None):
+        """
+               Pause for <time_in_sec>
+
+               :param time_in_sec:
+               :return:
+               """
+        self.wait_for_a_while(time_in_sec)
+
     def wait_for_a_while(self, time_in_sec=None):
         """
         Pause for <time_in_sec>
 
         :param time_in_sec:
         :return:
         """
```

### Comparing `nrobo-2024.37.0/nrobo/util/commands/ncommands/__init__.py` & `nrobo-2024.38.0/nrobo/util/commands/ncommands/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/commands/posix/__init__.py` & `nrobo-2024.38.0/nrobo/util/commands/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/commands/windows/__init__.py` & `nrobo-2024.38.0/nrobo/util/commands/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/common/__init__.py` & `nrobo-2024.38.0/nrobo/util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/constants/__init__.py` & `nrobo-2024.38.0/nrobo/util/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/database/connectors.py` & `nrobo-2024.38.0/nrobo/util/database/connectors.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/filesystem/__init__.py` & `nrobo-2024.38.0/nrobo/util/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/network/__init__.py` & `nrobo-2024.38.0/nrobo/util/network/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/platform/__init__.py` & `nrobo-2024.38.0/nrobo/util/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/process/__init__.py` & `nrobo-2024.38.0/nrobo/util/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/python/__init__.py` & `nrobo-2024.38.0/nrobo/util/python/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/regex/__init__.py` & `nrobo-2024.38.0/nrobo/util/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo/util/version/__init__.py` & `nrobo-2024.38.0/nrobo/util/version/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/nrobo.egg-info/PKG-INFO` & `nrobo-2024.38.0/nrobo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.37.0
+Version: 2024.38.0
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,113 +384,113 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 39.39%
-     - 22,502
+     - 39.34%
+     - 22,712
    * - CN
-     - 13.15%
-     - 7,511
+     - 13.09%
+     - 7,556
    * - DE
-     - 5.83%
-     - 3,330
+     - 6.10%
+     - 3,524
    * - SG
-     - 5.30%
-     - 3,025
+     - 5.28%
+     - 3,047
    * - RU
-     - 5.18%
-     - 2,962
+     - 5.19%
+     - 2,996
    * - HK
-     - 4.24%
-     - 2,420
+     - 4.21%
+     - 2,432
    * - JP
-     - 3.17%
-     - 1,810
+     - 3.15%
+     - 1,818
    * - FR
-     - 2.90%
-     - 1,657
+     - 2.88%
+     - 1,664
    * - KR
-     - 2.78%
+     - 2.75%
      - 1,589
    * - CA
-     - 2.73%
-     - 1,557
+     - 2.72%
+     - 1,569
    * - NO
-     - 1.99%
-     - 1,137
+     - 2.00%
+     - 1,155
    * - GB
      - 1.88%
-     - 1,072
+     - 1,085
    * - AU
-     - 1.79%
-     - 1,023
+     - 1.78%
+     - 1,027
    * - IN
      - 1.52%
-     - 869
+     - 879
    * - SE
      - 1.23%
-     - 702
+     - 708
    * - TH
-     - 0.80%
+     - 0.79%
      - 458
    * - HR
      - 0.79%
-     - 452
+     - 456
    * - DK
-     - 0.69%
+     - 0.68%
      - 395
    * - IE
      - 0.66%
-     - 375
+     - 381
    * - TW
-     - 0.64%
+     - 0.63%
      - 363
    * - IL
      - 0.56%
      - 321
    * - NL
-     - 0.52%
+     - 0.51%
      - 297
    * - ES
-     - 0.46%
+     - 0.45%
      - 262
    * - CH
      - 0.43%
-     - 244
+     - 246
    * - AE
      - 0.35%
-     - 201
+     - 203
    * - FI
      - 0.16%
      - 91
    * - ZA
-     - 0.16%
+     - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.11%
      - 61
-   * - TR
+   * - CW
      - 0.08%
      - 44
-   * - CW
+   * - TR
      - 0.08%
      - 44
-   * - IS
+   * - OM
      - 0.07%
      - 42
-   * - CZ
+   * - IS
      - 0.07%
      - 42
-   * - OM
+   * - CZ
      - 0.07%
      - 42
    * - RO
      - 0.04%
      - 24
    * - GF
      - 0.02%
@@ -509,20 +509,20 @@
      - 3
    * - EE
      - 0.01%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
-   * - MX
+   * - RS
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **57,129**
+     - **57,738**
```

### Comparing `nrobo-2024.37.0/nrobo.egg-info/SOURCES.txt` & `nrobo-2024.38.0/nrobo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.37.0/pyproject.toml` & `nrobo-2024.38.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools >= 40.7.0",]
 build-backend = "setuptools.build_meta"
 
 # Project details
 [project]
 name = "nrobo"
-version = "2024.37.0"
+version = "2024.38.0"
 authors = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 maintainers = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 description = "Powerful! Yet, Easy to USE! Automated Testing Framework"
 readme = "README.rst"
 keywords = ["test automation", "test automation framework", "automated testing", "automation testing", "testing", "qa", "acceptance test", "automation"]
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
```

