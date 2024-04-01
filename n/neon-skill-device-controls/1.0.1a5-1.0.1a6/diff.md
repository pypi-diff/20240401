# Comparing `tmp/neon-skill-device_controls-1.0.1a5.tar.gz` & `tmp/neon-skill-device_controls-1.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-device_controls-1.0.1a5.tar", last modified: Thu Feb  1 21:38:23 2024, max compression
+gzip compressed data, was "neon-skill-device_controls-1.0.1a6.tar", last modified: Mon Apr  1 21:53:53 2024, max compression
```

## Comparing `neon-skill-device_controls-1.0.1a5.tar` & `neon-skill-device_controls-1.0.1a6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.805997 neon-skill-device_controls-1.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-01 21:38:23.805997 neon-skill-device_controls-1.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    14983 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.789997 neon-skill-device_controls-1.0.1a5/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.789997 neon-skill-device_controls-1.0.1a5/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.793997 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/action_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/already_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/already_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/ask_disable_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/ask_exit_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/ask_start_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/ask_start_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_brain_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_brain_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_exiting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_listening_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_listening_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_require_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_skip_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_ww_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_ww_changing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/confirm_ww_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/error_invalid_ww_requested.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/error_no_ww_api.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/error_no_ww_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/error_ww_already_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/error_ww_change_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/dialog/not_doing_anything.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.797997 neon-skill-device_controls-1.0.1a5/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/intent/exit.intent
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/intent/restart.intent
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/intent/shutdown.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.797997 neon-skill-device_controls-1.0.1a5/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/regex/wakeword.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.797997 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/debug.voc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/disable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/enable.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/exit.voc
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/listening.voc
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/mycroft.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/no.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/request.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/restart.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/shutdown.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/solo.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/start.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/start_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/stop.voc
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/stop_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/en-us/vocab/ww.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.789997 neon-skill-device_controls-1.0.1a5/locale/uk-ua/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.801997 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/action_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/already_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/already_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/ask_disable_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/ask_exit_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/ask_start_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/ask_start_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_brain_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_brain_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_exiting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_listening_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_listening_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_require_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_skip_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_ww_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_ww_changing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/confirm_ww_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/error_invalid_ww_requested.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/error_no_ww_api.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/error_no_ww_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/error_ww_already_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/error_ww_change_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/dialog/not_doing_anything.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.801997 neon-skill-device_controls-1.0.1a5/locale/uk-ua/intent/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/intent/exit.intent
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/intent/restart.intent
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/intent/shutdown.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.801997 neon-skill-device_controls-1.0.1a5/locale/uk-ua/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/regex/wakeword.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.805997 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/debug.voc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/disable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/enable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/exit.voc
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/listening.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/mycroft.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/no.voc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/request.voc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/restart.voc
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/shutdown.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/solo.voc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/start.voc
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/start_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/stop.voc
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/stop_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/locale/uk-ua/vocab/ww.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.805997 neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-01 21:38:23.000000 neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-02-01 21:38:23.000000 neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 21:38:23.000000 neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-01 21:38:23.000000 neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-01 21:38:23.000000 neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-01 21:38:23.000000 neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 21:38:23.805997 neon-skill-device_controls-1.0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 21:38:23.805997 neon-skill-device_controls-1.0.1a5/test/
--rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-01 21:38:17.000000 neon-skill-device_controls-1.0.1a5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.870380 neon-skill-device_controls-1.0.1a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 21:53:53.870380 neon-skill-device_controls-1.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14983 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.854380 neon-skill-device_controls-1.0.1a6/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.854380 neon-skill-device_controls-1.0.1a6/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.858380 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/action_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/already_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/already_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/ask_disable_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/ask_exit_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/ask_start_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/ask_start_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_brain_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_brain_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_exiting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_listening_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_listening_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_require_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_skip_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_ww_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_ww_changing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/confirm_ww_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/error_invalid_ww_requested.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/error_no_ww_api.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/error_no_ww_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/error_ww_already_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/error_ww_change_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/dialog/not_doing_anything.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.858380 neon-skill-device_controls-1.0.1a6/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/intent/exit.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/intent/restart.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/intent/shutdown.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.858380 neon-skill-device_controls-1.0.1a6/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/regex/wakeword.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.862380 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/debug.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/disable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/enable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/exit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/listening.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/mycroft.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/no.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/request.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/restart.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/shutdown.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/solo.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/start.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/start_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/stop_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/en-us/vocab/ww.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.854380 neon-skill-device_controls-1.0.1a6/locale/uk-ua/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.866380 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/action_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/already_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/already_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/ask_disable_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/ask_exit_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/ask_start_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/ask_start_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_brain_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_brain_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_exiting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_listening_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_listening_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_require_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_skip_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_ww_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_ww_changing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/confirm_ww_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/error_invalid_ww_requested.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/error_no_ww_api.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/error_no_ww_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/error_ww_already_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/error_ww_change_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/dialog/not_doing_anything.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.866380 neon-skill-device_controls-1.0.1a6/locale/uk-ua/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/intent/exit.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/intent/restart.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/intent/shutdown.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.866380 neon-skill-device_controls-1.0.1a6/locale/uk-ua/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/regex/wakeword.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.870380 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/debug.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/disable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/enable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/exit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/listening.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/mycroft.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/no.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/request.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/restart.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/shutdown.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/solo.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/start.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/start_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/stop_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/locale/uk-ua/vocab/ww.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.870380 neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 21:53:53.000000 neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-01 21:53:53.000000 neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:53:53.000000 neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 21:53:53.000000 neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 21:53:53.000000 neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 21:53:53.000000 neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:53:53.870380 neon-skill-device_controls-1.0.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:53:53.870380 neon-skill-device_controls-1.0.1a6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-01 21:53:48.000000 neon-skill-device_controls-1.0.1a6/version.py
```

### Comparing `neon-skill-device_controls-1.0.1a5/LICENSE.md` & `neon-skill-device_controls-1.0.1a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.0.1a5/PKG-INFO` & `neon-skill-device_controls-1.0.1a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-device_controls
-Version: 1.0.1a5
+Version: 1.0.1a6
 Home-page: https://github.com/NeonGeckoCom/skill-device_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-device_controls-1.0.1a5/README.md` & `neon-skill-device_controls-1.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.0.1a5/__init__.py` & `neon-skill-device_controls-1.0.1a6/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/PKG-INFO` & `neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-device-controls
-Version: 1.0.1a5
+Version: 1.0.1a6
 Home-page: https://github.com/NeonGeckoCom/skill-device_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-device_controls-1.0.1a5/neon_skill_device_controls.egg-info/SOURCES.txt` & `neon-skill-device_controls-1.0.1a6/neon_skill_device_controls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.0.1a5/setup.py` & `neon-skill-device_controls-1.0.1a6/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.0.1a5/skill.json` & `neon-skill-device_controls-1.0.1a6/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.0.1a5/test/test_skill.py` & `neon-skill-device_controls-1.0.1a6/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.0.1a5/version.py` & `neon-skill-device_controls-1.0.1a6/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a5"
+__version__ = "1.0.1a6"
```

